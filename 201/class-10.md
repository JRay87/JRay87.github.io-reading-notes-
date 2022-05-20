# ***Day 10** - The only "good" bug is a De-bug*

## ***JS Chapter 10** - Error Handling & Debugging*

JavaScript is very difficult to write correctly the first time. More often than not you will have errors in your code. Debugging is a great way to find and fix the errors in your code. 

First thing to remember is that code is read in order top down so understanding the order of exectution for your code you can track the error back to its root cause. 

JavaScript interpreter uses "execution contexts" which states that every statement in code is one of three types:

- Global Context - Only one in page, not in a function

- Function Context - code run in a function

- Eval Context - Evaluates code with text

JavaScript stacks functions on top of eachother, newest on top.

Whenever script enters a new execution context is goes through two phases: Prepare (takes the functions/variables and hoists them to the top of the execution context) and Execute (runs the code).

Functions have lexical scope (attached to the function they were written in). Execution contexts means that they have access to the variables object, plus any parent object.

All of this information can help developers track down and fix bugs in the code. There are many differrent types of errors and can be found *p459-461*.

To properly and efficiently debug your code you should inspect the console and look at the (if any) error code. This will usually hold vital information like where the error is initiaing and any other iterations that are having errors caused by the initial. Once you find what the issue is you can look at what is actually causing the error. Breaking down what you wrote can help you figure out what you are trying to do which can help figure out how you went wrong. 

Inside the console you can call functions to ensure that they run properly or can summon variables. It can also help if you write console logs into the code to make sure that it is running as desired and comes up with the values you are expecting. You can also console a table for data that would look better displayed in a table.

Other tricks you can use include breakpoints which stop the code at a specific point so you can check the values stored in the variables. If you make mutliple you can *step* through them to see point by point how the code is operating.(You can even set conditional breakpoints.) 

Placing the keyword `debugger` in the code will make a breakpoint.

Another option can be `try`, `catch`, and `finally`.

- Try - if an exception occurs control is passed to the catch.

- Catch - this is a different piece of code that will run if the first causes an error. 

- Finally - will run whether or not an exception was found in the try block.

Last option described in the book was throwing errors which allows the developer to recognize an error before the system does such as a string value vs number. 