## SMACSS and Responsive Web Design

### Responsive Web Design

* "Responsive web design is the practice of building a website suitable to work on every device and every screen sizes, no matter how large or small, mobile or desktop."
* **Responsive** and **adaptive** design are closely related
  * Responsive sites continually and fluidly change based on different factors such as viewport width
  * Adaptive sites are built to a group of preset factors
  * Using the two in combination is ideal
* **Mobile** design generally means building a separate site specifically for use on a mobile device. Not efficient
* RWD (responsive web design) has three main components
  * **Flexible Layouts**
    * Avoid using fixed measurements but rather use percentage or ems
    * CSS3 offers viewport sizse units such as `vw, vh, vmin, vmax`
    * Obtain the relative width of an element by taking the target width and dividng by the width of the parent element
    * Applying flexible grid concepts to all parts of a site create a completely dynamic site, scaling to every viewport size
  * **Media Queries**
    * Provide the ability to specify different styles for individual browsers and devices
    * It is most commmon to intialize media queries within the CSS file like this:
      * `@media`
    * Three logical operators for use in media queries
      * `and, not, only`
    * The **and** operator allows for multiple conditions to be used
    * The **not** operators negates the query
    * The **only** operator limits the media query to what device is specified
    * One of the most common media features revolves around determining a height or wdith for a browser
      * Specify `min-width` and `max-width` to build responsive websites on desktops and mobile devices equally
    * **orientation** allows for adjustment based on landscape or portrait presentation
    * Mobile First is a concept that starts with mobile web design, and only adds features for larger devices when necessary. 
      * Advocates designing with the constraints of a mobile user in mind
      * This saves bandwidth for the majority of people who are consuming things on their mobile devices first
    * Using the viewport **meta** tag with height or width values defines the height or width of the viewport respectively
    * **Viewport scale** is from 0-10, with 1 being the most commong starting point. 
      * Use `initial-scale` to specify viewport scale
  
* **Flexible Media**

* Flexible media allows images, videos an other media types to flex and change along with the size of the viewport.
* It can be difficult for embedded media such as iFrames to flex
  * this requires additional layout rules
  * Position the embedded media absolutely within the parent element and make sure parent element has width of 100% in order to scale based on the width of the viewport
  * Parent element also must have height of 0 
  * Example: 
  `figure {
  height: 0;
  padding-bottom: 56.25%; /* 16:9 */
  position: relative;
  width: 100%;
}
iframe {
  height: 100%;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
}`


### All About Floats

* **Float** is a CSS positioning property that allows content such as text to flow around the floated element.
  * Content flowing around an element is called Text-Wrap
* Floated elements remain a part of the flow of a web page
  * This is different than absolutely positioned elements, which are removed from the flow of a page
* There are four vlaues for the float property
  * Left, right, none (default) and inherit (inherits parent element float property)
* Floats can be used to design layout, or simply positioning an element such as a photo within a containing element
* **Clear** allows elements to ignore the float element and be positioned below, rather than wrapping up around the floated element. 
  * Clear allows for left, right, both or none
* When floating, parent elements collapse if they contain nothing but floated elements.
  * This can be fixed by clearing the float after the floated elements, prior to the close of the container
  * There are several ways to clear floats
    * Create an empty <div> container
    * Use `overflow` on the parent element
    * Use CSS selector `:after` to clear the float
* Floats are considered fragile

### Don't Overthink It Grids

* Grids can be simple using columns with percentage widths and the `float` property
* Try using `border-box` which maintains the width of a box despite the addition of padding or borders


### CSS Floats Explained By Riding An Escalator

* Float elements create two lines, such as an escalator. It allows for content to flow on both the rigth and left of the containing element, making design much more fluid




