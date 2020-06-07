### Node, Express, and APIs

#### An Introduction to Node.js on sitepoint.com

* What is Node.js?
  * Built on Google Chrome's V8 JavaScript Engine
    * V8 is an open-source engine
    * Designed with performance in mind
  * Not executed in a browser
  * A JavaScript runtime

* Installing Node.js
  * It is suggested to use a version manager instead of the direct website download
  * Allows you to install multiple versions of Node and switch between them
  * Version manager negates potential permission issues when using Node with npm and lets user set a Node version on a per-project basis

* Proof of Life
  * Confirm proper installation by opening terminal and typing `node -v`. A version should return
  * Next, create a `hello.js` file and console log 'Hello World'.

* Support for Modern JavaScript
  * Excellent support for ECMAScript and beyond
  * Very few compatibility issues

* NPM - JavaScript Package Manager
  * Check version by typing `npm -v`
  * World's largest software registry
  * Install globally - `npm install -g jshint`
  * Install locally - `init y`

* Working with package.json File
  * node_modules is where npm saves `lodash` and any libraries `lodash` depends on 
  * Can be re-created at any time by running `npm install` from project root
  * Specifying project dependencies allows any developer to clone project and use npm to install necessary packages

* Uses for Node.js
  * Installing (via npm) and running (via node) build tools designed to automae the process of developing a modern JavaScript application
  * Build tools come in all shapes and sizes
  * Build tools can be used for anything from bundling JavaScript files and dependencies to running test

* Node.js allows users to run JavaScript on the server
  * Node.js is single-threaded and event-driven, so everything that happens in Node.js is in reaction to an event. This causes the server very little overhead and is capable of handling a large number of simultaneous connections

* Advantages of Node.js
  * Speed
  * Scalability
  * no longer necessary to switch modes
    * Everything can be done in the same language
  * Speaks JSON. 
    * Most important data exchange format on the web
  * JavaScript is ubiquitous - Most are familiar with it so the transition to Node development is potentially easier