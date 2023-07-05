# Readings: In memory storage

## Javascript Error Messages

* The article discusses common types of errors in JavaScript and provides explanations and examples for each type. The types of errors covered are:

1. Reference errors: Occur when you try to use a variable that is not yet declared.
2. Syntax errors: Arise when there is a problem with the syntax of the code.
3. Range errors: Happen when an object with a length property is manipulated with an invalid length.
4. Type errors: Occur when incompatible types are used or accessed, such as accessing a property of an undefined variable.

* The article also covers the process of debugging JavaScript code. It suggests using techniques like console.log() statements, breakpoints in browser developer tools, and conditional breakpoints for more complex scenarios. It highlights the importance of the call stack in understanding the flow of execution and provides examples of how to leverage it for debugging purposes.

* Additionally, the article touches on handling errors and suggests using try...catch blocks to catch and handle errors gracefully, preventing them from crashing the application. It emphasizes the importance of proper error handling to ensure the application can recover from errors and continue functioning.

* The article concludes by mentioning some tools that can help developers in avoiding runtime errors, such as quokka for evaluating code as you type and ESLint for enforcing code style and catching errors.

* Overall, the article provides an overview of common JavaScript errors, debugging techniques, and error handling practices. It aims to help developers improve their ability to read error messages, debug code effectively, and build more robust applications.

### Error Questions

1. Reference Error: A reference error occurs when you try to use a variable or function that hasn't been declared or defined. It indicates that the interpreter or compiler cannot find a reference to the specified identifier.

2. Syntax Error: A syntax error occurs when the code violates the rules of the programming language's syntax. It means the code is not written correctly according to the grammar and structure expected by the language. Syntax errors typically prevent the code from being executed.

3. Range Error: A range error occurs when a value is not within an acceptable range or set of values. For example, it could happen when trying to access an array element with an index that is out of bounds or when using a number that is outside the valid range for a specific operation.

4. Type Error: A type error occurs when an operation is performed on a value of an inappropriate type. It indicates that the code is trying to use a value or perform an operation that is not compatible with the data type or object being used.

5. Breakpoint: A breakpoint is a debugging feature provided by programming tools and environments. It allows you to pause the execution of your code at a specific line or condition, enabling you to inspect the program's state and values at that point.

6. Debugger: A debugger is a tool or software feature used during the development and testing of code to identify and fix errors or bugs. It allows programmers to step through their code, set breakpoints, inspect variables, and observe the program's execution in detail. A debugger helps in understanding and resolving issues by providing a controlled environment for code analysis and debugging.

## Call Stack

* Call Stack: The call stack is a data structure that follows the Last In, First Out (LIFO) principle to manage function invocation. It is a single-threaded interpreter comprising a heap and a single call stack.

* Synchronous Execution: The call stack executes functions synchronously, one at a time, from top to bottom. The last function pushed into the stack is the first to be popped out when it returns.

* Temporary Storage: When a function is invoked, its parameters and variables are pushed into the call stack to create a stack frame. This stack frame is a memory location in the stack, and it is cleared when the function returns.

* Managing Function Invocation: The call stack keeps track of the position of each stack frame and knows the next function to be executed. This allows for the synchronous execution of code in JavaScript.

* Recursive Functions and Stack Overflow: A stack overflow occurs when a recursive function doesn't have an exit point, causing the call stack to exceed its maximum capacity. This results in an error being thrown, such as "Maximum call stack size exceeded."

* The understanding of the call stack is crucial for grasping asynchronous programming concepts, which will be covered in future articles.

* Overall, the call stack in JavaScript plays a fundamental role in managing function execution and maintaining the order of operations within the program.

### Questions for Call stack

1. In programming, a "call" refers to the action of invoking a function or method. When a function is called, the program jumps to that function's code and executes it, and once the function completes its execution, the program returns to the point where the function was called from.

2. The number of "calls" that can happen at once depends on the programming language and the execution environment. In general, most programming languages allow multiple function calls to happen concurrently through mechanisms like multi-threading or asynchronous programming. However, the specific limitations and concurrency capabilities vary across languages and runtime environments.

3. LIFO stands for "Last-In, First-Out," which is a principle commonly associated with data structures like stacks. In the context of a call stack, LIFO means that the most recent function call that was made will be the first one to be completed and returned, followed by the next most recent one, and so on.

4. Here's an example of a call stack with multiple function invocations:

* function main() {
  console.log("In main");
  functionA();
}

* function functionA() {
  console.log("In functionA");
  functionB();
}

* function functionB() {
  console.log("In functionB");
}

* main();


* Call stack:
main()
functionA()
functionB()

Each function call adds a new frame to the top of the call stack, and when a function completes, its frame is removed from the stack, allowing the program to continue executing the remaining functions.

5. A stack overflow occurs when the call stack exceeds its maximum size or capacity. This can happen due to recursive function calls that don't have proper termination conditions or excessive nested function invocations. When a stack overflow occurs, it means that the call stack has run out of available space, and the program is unable to handle additional function calls. This results in an error, commonly known as a "stack overflow error" or "stack overflow exception."
