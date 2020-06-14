### EJS

### Intro to EJS

#### Getting Started

* DB Congig - easy way to build out
* npm init -y
* npm install --save express body-parser cors ejs
* var express = require('express);
* var bodyparser = require('bodyparser');
* var cors = require('cors');
* var path = require('path');
* var app = express();
* app.use(bodyparser());
* app.use(cors());
* app.set('views', path.join(_dirname, 'views'));
* app.set('view engine', 'ejs');

* Create new views folder
  * index.ejs

* app.get('/', function (request, response) {
  response.render('index', {
    foo: 'bar';
  });
}

* app.listen(8000, function() {
  console.log('heard on 8000');
})

#### Injecting Values into EJS view

* Response.render - three parameters

* Equals sign evaluates a variable (=)
* <> - opening and closing EJS tags
* "<%= foo %>"


### Google Books API Docs

* Google Volumes API request URL
  * https://www.googleapis.com/books/v1/volumes?q=search+terms
  * Add text strings to search in particlular fields such as **intitle** or **inauthor**
* Add other query parameters to filter only for books that are available for download (epub)
  * Other Examples - partial, full, free-ebooks, paid-ebooks.
* **Pagination** - Limit amount returned
* **Print Type** - Filter for a specific print or publication type
* **Projection** - Redefined set of volumes returned
* **Sorting** - **Orderby** to change order
* **Projection** - Return full or lite volumes

* Retrieve a User's public bookshelves
  * https://www.googleapis.com/books/v1/users/userId/bookshelves
  * No authorization HTTP needed since public
* Retrieve list from "my" library
  * https://www.googleapis.com/books/v1/mylibrary/bookshelves



### EJS Docs

* What is EJS? - Template language that lets you generate HTML markup witih plain javascript
* Embedded JavaScript Templating
* Use Plain JavaScript
* Fast Development Time
* Simple Syntax
* Quick execution
* Easy to debug
* Ongoing development
* Install - npm install ejs

### EJS Tutorial

* **partials** - Code that is reused
* Syntax - `<% include FILENAME %>`
* 


