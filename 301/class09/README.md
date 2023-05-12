# Functional Programming

Functional programming is a programming paradigm that emphasizes on the use of pure functions, which are functions that have no side-effects and always return the same output for the same input.

Some of the key concepts of functional programming in JavaScript are:

* Immutability: In functional programming, data is immutable and cannot be changed. Instead of changing data, new data is created. This is achieved by using techniques such as copying objects or arrays before modifying them, and returning new objects or arrays from functions instead of modifying existing ones.

* Higher-order functions: Functions that take other functions as arguments, or return functions, are called higher-order functions. They are a key concept in functional programming because they enable the creation of more modular and reusable code.

* Pure functions: Pure functions are functions that have no side-effects and always return the same output for the same input. They are a key concept in functional programming because they enable code that is easier to reason about, test, and debug.

* Recursion: Recursion is a technique where a function calls itself repeatedly until a certain condition is met. It is a key concept in functional programming because it enables the creation of elegant and concise solutions to complex problems.

* Function composition: Function composition is the technique of combining two or more functions to create a new function. It is a key concept in functional programming because it enables the creation of more complex functions by combining simpler ones.

In JavaScript, functional programming is supported by features such as arrow functions, the spread operator, the rest parameter, and higher-order functions such as map, reduce, and filter.

### Questions Programming Concepts

1. Functional programming is a programming paradigm that focuses on using pure functions and immutable data structures to write programs. The key idea of functional programming is to treat computation as the evaluation of mathematical functions and avoid changing state and mutable data.
2. A pure function is a function that always returns the same output for a given input and has no side effects on the program or the environment. A function can be considered pure if it does not modify its arguments, it does not use mutable data, and it does not have any side effects like writing to a file or modifying a global variable. In other words, a pure function is idempotent, meaning it produces the same result no matter how many times it is called with the same arguments.
3. The benefits of pure functions are many. Because they always return the same output for a given input, pure functions are predictable and easier to reason about. They are also easier to test because they do not rely on external state or mutable data. Finally, pure functions can be composed together to build more complex functions, making it easy to reason about the behavior of the code.
4. Immutability is the property of data that cannot be modified after it has been created. In functional programming, immutable data structures are preferred because they can be shared safely between different parts of the program without the risk of unintended modifications. Because the data is immutable, it can be passed around freely, which reduces the need for copying and can improve performance.
5. Referential transparency is a property of pure functions that guarantees that the function can be replaced with its return value without affecting the behavior of the program. This means that the function can be replaced with a constant value, which can simplify reasoning about the code and can also improve performance by allowing the compiler to optimize the code.

## Modules and Require()


* A module is a reusable piece of code that can be used in other applications.
* In Node.js, each file is treated as a module and can be used in other files using the require() function.
* The require() function is used to load a module in Node.js. It takes the name of the module as a parameter and returns the module's exports object.
* To create a module in Node.js, you need to define the code you want to export from the module using the exports object.
* You can export a function or an object from a module by setting it as a property of the exports object.
* To use a module in another file, you need to require() it and assign the returned exports object to a variable.
* You can use the properties and methods of the exports object to access the functionality provided by the module.
* You can also create a module that exports multiple functions and objects by setting them as properties of the exports object.
* You can also require built-in Node.js modules, third-party modules, and local modules in your application using the require() function.
* The require() function searches for modules in the following order: built-in Node.js modules, local modules, and third-party modules installed in the node_modules folder.
* You can install third-party modules in your application using the npm package manager.

### Questions on module and require 

1. A module is a reusable piece of code that can be used in other applications.
2. The require() function is used to load a module in Node.js. It takes the name of the module as a parameter and returns the module's exports object.
3. To bring another module into the file that we are working in, we use the 'require' function and pass the path to the module as an argument. The path can be a relative or absolute path to the module file.
4. To make a module available, we need to export the functions, classes or objects that we want to make available from the module. We can do this by assigning the functions, classes or objects to the module.exports object. Once we export the functions, classes or objects, we can use the 'require' function to load the module in other parts of our application.




