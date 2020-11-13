# The Call Stack and Debugging

## The Call Stack defined on MDN
- A *call stack* is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.
- When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
- Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
- When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
- If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.
- **Summary: we start with an empty call stack. Whenever a function is invoked, it is automatically added to the call stack. Once the function has executred all of its code, it is automatically removed from the call stack. The call stack is now empty again.**

## The Javascript Call Stack- What It Is and Why It's Necessary: Charles Freeborn
- The JavaScript engine (which is found in a hosting environment like the browser), is a single-threaded interpreter comprising of a heap and a single call stack. The browser provides web APIs like the DOM, AJAX, and Timers.
- The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.
- In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.
- At the most basic level, a *call stack* is a data structure that uses the Last In, First Out (**LIFO**) principle to temporarily store and manage function invocation call.
- **Temporarily store**: When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack.
- **Manage function invocation (call)**: The call stack maintains a record of the position of each stack frame. It knows the next function to be executed and will remove it after execution,this is what makes code execution in JavaScript synchronous.
- A **stack overflow** occurs when there is a recursive function (a function that calls itself) without an exit point. The browser has a maximum stack call that it can accomodate before throwing a stack error.
- **Key Takeaways from the call stack:**
- It is single-threaded. It can only do one thing at a time
- Code execution is synchronous.
- A function invocation creates a stack frame that occupies a temporary memory
- It works as a *LIFO* (Last In, First Out data structure)
## Javascript error messages && debugging- Diogo Spinola
- *Green* error is the overall error message
- *Light blue* is to note if the error was properly handled
- *Brownish(dark yellow)* is the type of error 
- *Red* is the call stack
- **Types of error messages**:
- The first indication something is wrong in your code is the error message.
- *Reference errors* this is as simple as when you try to use a variable that is not yet declared 
- This is also a common thing when using const and let, they are hoisted like var and function but there is a time between the hoisting and being declared so when you try to access them a reference error occurs, the fact that this happens to let and const is called Temporal Dead Zone (TDZ).
- Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.
- This is probably the most frequent error in JS, trying to access a property/method thinking that bar is of the type object when in reality, since it hasn’t been declared yet, it’s undefined which doesn’t have any baz available.
- The fix is simply making sure *bar* exists before trying to access it.


