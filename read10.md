### The Call Stack and Debugging

#### Call Stack Defined

* Mechanism for an interpreter to keep track of its place in a script that calls multiple functions
  * Interpreter adds a function to the call stack when the script is called
  * Any functions within that function are added to the stack further up and run when their call is reached
  * When the current function is complete, the interpreter takes it off the stack and resume execution
  * If the stack takes up more space than is assigned to it, a "stack overflow" error occurs

  #### Understanding the JavaScript Call Stack

  * JavaScript engine is found in a hosting environment such as a browser

  * Call Stack is synchronous, meaning functions are executed one at a time
  * With asynchronous JavaScript, there is a callback function, an event loop, and a task queue. 
  * The callback funcion is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.
  * Call Stacks use the Last In, First Out (LIFO) principle
  * When a function is invoked, the function, parameters and variables created a stack frame. It is a memory location in the stack. That memory is cleared when the function returns
  * Stack overflow occurs when a fuction calls itself without an exit point

### JavaScript Error Messages

* Reference Errors - 
  * **Temporal Dead Zone** - When trying to use a variable that is not declared
    * Fix by declaring the variable before any declaration is made
* Syntax Errors - Fix the error, such as a missing paren
* Range Errors
  * Giving an object an invalid length
    * Example - An array cannot have a negative length
* Type Errors - Incompatibility, such as accessing a property in an undefined type of variable
  * One of the most common errors

* Debugging Code
  * console.log is the easiest and most common
  * Add breakpoints to see if code before a certain point is running properly
  * 
