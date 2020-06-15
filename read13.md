### Update/Delete

#### Sending Form Data

* What happens whena user submits a form?
  * Where does the data go and how is it handled?


* At its most basic, a client (usually a browser) sends a request to a server using HTTP protocol, and the response uses the same protocol. 
* An HTML form is a convenient, user-friendly way to configure an HTTP request to send data to a server
* The `<form>` element defines how the data will be sent
  * `action` and `method` are the most important attributes

* **Action** - Defines where the data gets sent
  * Value must be valid relative to the absolute URL
  * Names and values of the non-file form controls are sent as name/value pairs
  * The action value needs to be a file on the server that can handle the incoming data
  * The server then responds by handling the data and loading the URL defined by the action attribute, causing a new page to load

* **Method** - Defines HOW the data is sent
  * The HTTP protocol provides several ways to perform a request, using methods such as **GET** or **POST**
  * How does this work? 
    * Each time you want to reach a web resource, the browser sends a request to a URL. 
    * An HTTP request consists of a **header** that contains a set of global metadata about the browser, and a **body** that contains information necessary for the server to process the specific request

* **GET** - Hey server, I want to get this resource
* **POST** - Hey server, take a look at this data and send back to me an appropriate result
  * The same submission using post does not append data to the URL

* HTTP requests are never displayed to the user
  * You can view form submission details in developer tools
  * The only thing displayed to the user is the URL called
  * With the GET method, the user will see their data in the URL call, but not with the POST method
  * Do not use the GET method when sending sensitive information
  * Use POST to send large amounts of data

#### Retrieving Data - Server Side

* Server receives a string that will be parsed in order to get the data as key/value pairs
* **PHP** - General purpose scripting language
* **Python** - Use the **Flask Framework**
* Other server-side technologies used for handling data include **Java**, **.Net**, **Ruby**

* Sending files with HTML forms is a special case. 
  * Files are binary data, whereas all other data is text data
  * Since HTTP is a text protocol, there are special requirements for handling binary data

  * Use the **enctype** attribute
    * Method - POST
    * Value - enctype
    * Include one or more `<input type="file">`

* Never trust your users - be paranoid
  * Escape potentially dangerous characters
  * Limit amount of incoming data to allow only what's necessary
  * Store on different server and allow access ot the file only through a different subdomain - **sandbox uploaded files**



#### HTML5 Forms Reference

* **Action** - Defines which URL the form's information is sent to when submitted
  * Use relative URL or absolute URL

* **Method** - Defines the HTTP method used when submitting the form
  * **POST** - The form information is sent to the server as part of the request body
  * **GET** - The form information is sent to the server as part of the URL parameters