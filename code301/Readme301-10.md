# THE CALL STACK

A call stack is a mechanism for an interpreter to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.



call stack is primarily used for function invocation, Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom.


At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.


Temporarily store: When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack.

Manage function invocation (call): The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.



1. When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.

2. Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.

3. When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.

4. If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

### Example

function greeting() {
   // [1] Some code here
   sayHi();
   // [2] Some code here
}

function sayHi() {
   return "Hi!";
}

// Invoke the `greeting` function
greeting();

// [3] Some code here


The code above would be executed like this:

Ignore all functions, until it reaches the greeting() function invocation.

Add the greeting() function to the call stack list.

Call stack list:
- greeting

Execute all lines of code inside the greeting() function.

Get to the sayHi() function invocation.

Add the sayHi() function to the call stack list.

Call stack list:
- sayHi
- greeting

Execute all lines of code inside the sayHi() function, until reaches its end.

Return execution to the line that invoked sayHi() and continue executing the rest of the greeting() function.

Delete the sayHi() function from our call stack list.

Call stack list:
- greeting

When everything inside the greeting() function has been executed, return to its invoking line to continue executing the rest of the JS code.

Delete the greeting() function from the call stack list.

Call stack list:
EMPTY



In summary, then, we start with an empty Call Stack. Whenever we invoke a function, it is automatically added to the Call Stack. Once the function has executed all of its code, it is automatically removed from the Call Stack. Ultimately, the Stack is empty again.

![call stack](https://github.com/naeemmusamh/Reading-note/blob/master/IMAGE/call%20stack.jpg?raw=true)