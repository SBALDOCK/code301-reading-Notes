### EJS Partials

* Embedded JavaScript Templates
* **Partials** are built to be reused over multiple HTML views
* They can be considered functions and make larger websites easier to maintain
* Instead of changing a piece of text on every page it appears in, define reusable bundleds of code and include file wherever you need it.

* Partial tags look like this - `<%- include(File Name) %>`
* The `<%-%>` tags allow output of unescaped content on the page. Especially important when using the `-include` in the statement so the opening/closing tags aren't escaped


* Partials are native to EJS
* Nav bar, footer, reusable piece of static text
* Build EJS files and simply link them in HTML file
* `<h1>we can see you...most likely</h1>`
* Very very simple
