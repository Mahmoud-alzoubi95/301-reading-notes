# Read 10 : THE CALL STACK

Definition:

A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.


Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.


When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.


If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.


## The JavaScript Call Stack - What It Is and Why It's Necessary

The understanding of the call stack is vital to Asynchronous programming (which we will look at in a later article).

In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.


At the most basic level, a call stack is a data structure that uses the **Last In, First Out** (LIFO) principle to temporarily store and manage function invocation (call).

## JavaScript error messages && debugging

Types of error messages

1. Reference errors

a variable that is not yet declared

2. Syntax errors

this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

3. Range errors

Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

```
var foo= []
foo.length = foo.length -1 // Uncaught RangeError: Invalid array length
```

4. Type errors

this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.



# The End

