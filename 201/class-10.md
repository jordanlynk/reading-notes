# Ch.10 "Error Handling & Debugging"

- The console.log method can write several values to the console at the same time, each seperated by a comma.
- There are three different types of console methods, refer to page 472
- If you want to write a set of related data to the console, you can use the console.group() method to group the messages all together.
- In browsers that support it, the console.table() method allows you to output a table showing a) objects b) arrays that contain other objects or arrays
- Using the console.assert() method, you can test if a condition is met, and write to the console only if the expression equals to false
- You can create a breakpoint in your code using just the debugger keyword. When the developer tools are open, this will automatically create a breakpoint.
- If you understand excecution contexts, and stacks you are more likely to find error in your own code
- Debugging is the process of finding errors. It involves a process of deduction
- The console helps narrow down the area in which the error is located, so you can try to find the exact error
- JS has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error
- If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use these to give your users helpful feedback