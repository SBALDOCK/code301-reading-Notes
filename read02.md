### JavaScript and JQuery

* JQuery is a JavaScript file that is included in web pages that allows users to find elements using CSS-style selectors and then do something with the elements
* jQuery is a function that creates a jQuery "Object"
* The jQuery object has one parameter, which is a CSS-style selector:
  Example: `$('li.hot')` finds all <li> elements with the class "hot"
* After creating a jQuery object, add methods to perform changes or retrieve contents
  Example: `$(li.hot').addClass('complete');`
  * This adds the class "complete" to all <li> elements with the class "hot"

* jQuery does not require fallback code as it has cross-browser support
* It is most common to include a `<script>` element near the bottom of the <body> to allow the page to load fully, just like using JavaScript
* It is possible to add multiple methods using dot notation. This is called **chaining**
  Example: `$('li:lt(3)').hide().fadeIn(1500);` 
  * This example selects the first three list items and performance two methods - hides them, and then fades them in
* Select elements using CSS-style selectors.
  * jQuery provides some additional selectors that are unique to jQuery as well such as
    * not(selector)
    * :first
    * :last
    * :event
    * :odd
* Using `.html` retrieves information from just the first element in a matched set
  Example: `var content = $('li').html();` retrieves the contents from just the first <li> in the set
* jQuery objects store references to elements and can be cached in variables for future use

* It is possible to perform the same action on multiple elements withouth a loop as you can update all elements using a single method
* Use `.ready` to check if a page is ready to work with 
  Short example: `$(function() {//script goes here});`
* Retrieve all html content from the first element in a matched set with `.html`
  Example: `$('ul').html();`
* Retreive all text content from all elements using `.text`
  Example: `$('ul').text();`

* Use `.html`, `replaceWith`, `.text` or `.remove` to update elements with new content
* Insert new elements in two steps
  * Create new element
    * `var name = $('<li>');`
  * Use method to insert
    * `$('ul').before(element and content);`

* Add, access and update attributes using the following four methods
  * `attr()` - get or set a specified attribute and value
  * `removeAttr()` - remove a specified attribute
  * `.addClass()` - add a new value to existing class value
  * `.removeClass()` - remove a value from the class attribute

* Get a CSS property 
  * `var backgroundColor = $('li').css('background-color');`
* Set a CSS property
  * `$('li').css('background-color', '#272727');`
* Set multiple propertys through object literal notation

* Create the functionality of a loop on a select of elements using `.each`
  Example: `$(function(){ $('li').each(function()) var ids = this.id; $(this).append(' <span class="order">' + ids + '</span>'); }); });`

* Use `.on()` to handle all events
  * Example events are **focus**, **click**, **blur**, and **load**

* You can load jQuery from a CDN (content delivery network) with a backup `<script>` element to check whether the CDN script has loaded, and to run the jQuery script from the same server as the rest of the website









### 6 Reasons for Pair Programming

* Pair programming fosters a collaborate environment and reflects the workplace
* Pair programming general involves a drive and navigator
  * The driver is the programmer
  * The navigator is guiding the driver through words
* Pair programming exercises the four fundamental skills that help people learn a new language
  * Listening, speaking, reading, writing
* 1. Greater efficiency
  * Research a problem and a solution faster
  * Create higher-quality code
* 2. Engaged Collaboration
  * More engaging when two individuals focus on the same code
  * Two people rely more on each other and have to call for help less often
* 3. Learning from fellow students
  * Each indivdual has a different approach and they can learn tips and tricks from one another
  * Often times two coders have different skill sets, so each can teach the other something
* 4. Social skills
  * Learn how to interact with others
  * Communication is key
* 5. Job Interview readiness
  * Many interviews involve pair programming between an employee and an applicant. 
  * Pair programming prepares the coder for this
* 6. Work environment readiness
  * Companies use pair programming to train fresh hires 
  * Code Fellows graduates can hit the ground running since they are already familiar with it 