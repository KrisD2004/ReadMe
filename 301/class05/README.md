# Putting it all together

## Thinking in React

* Break down the UI into a component hierarchy: Before you start writing code, break down the UI into smaller, reusable components. Think about how you can divide the UI into smaller parts, and what data each component needs to render.

* Build a static version of the UI: Start by building a static version of the UI using only props and stateless functional components. This will help you think about the data flow and how to compose components.

* Identify the minimal state needed: Identify the minimal set of mutable state that your app needs. Determine which component should own each piece of state.

* Determine where your state should live: Once you've identified the minimal state needed, determine which component should own each piece of state. The component that renders a particular piece of data should be the one that owns and updates that data.

* Add inverse data flow: Sometimes a child component needs to update the state of its parent. To achieve this, pass down a function from the parent as a prop to the child, and have the child call that function when it needs to update the state of the parent.

* Think about the data flow: Think about how data flows through your app. Use the "top-down" approach, where state is passed down through props and actions are passed up through callbacks.

* Keep components small and focused: Each component should do one thing and do it well. Keep components small and focused on a specific task. If a component becomes too large, break it down into smaller components.

* Use props and state sparingly: Only use props and state when necessary. Use props for data that doesn't change, and state for data that does change. Avoid duplicating state in multiple components.

* Use React DevTools: Use the React DevTools to debug your components and understand the data flow.

* Test your components: Test your components to ensure they work as expected. Use tools like Jest and Enzyme to write unit tests for your components.

## Higher-Order Functions

* Functions can be values: In JavaScript, functions are treated as values just like strings or numbers. They can be stored in variables, passed as arguments to other functions, and returned as values from functions.

* Higher-order functions: A higher-order function is a function that operates on other functions, either by taking them as arguments or by returning them as values. Higher-order functions can be used to create abstraction and modularity in code.

* Functions that create new functions: Functions can be used to create new functions, such as the repeat function that takes a function and a number and returns a new function that calls the original function multiple times.

* Functions that change other functions: Functions can be used to modify other functions, such as the unless function that takes a condition and a function, and returns a new function that calls the original function only if the condition is false.

* Filtering arrays: The filter method can be used to create a new array that contains only the elements of the original array that pass a given test.

* Transforming with map: The map method can be used to create a new array that contains the result of calling a function on each element of the original array.

* Reducing with reduce: The reduce method can be used to accumulate a single value by repeatedly calling a function on each element of an array.

* Composability: Higher-order functions can be composed to create complex operations from simple building blocks.

* Abstraction: Higher-order functions can be used to abstract away the details of an operation, making code more modular and easier to understand.

## Question for thinking in react

1. The single responsibility principle (SRP) is a software design principle that states that a component or module should have only one reason to change. In other words, a component should have only one responsibility or job to do, and any changes to that responsibility should only affect that component. When it comes to components, the SRP means that each component should have a clear and specific responsibility, and it should not be responsible for multiple tasks or concerns. This makes components more modular, easier to understand, and easier to maintain.
2. Building a 'static' version of your application means creating a version of your application that doesn't require any server-side processing or dynamic data.
3. Once you have a static application, you need to add server-side processing and dynamic data in order to create a fully functional web application
4. To determine if something is state, you can ask three questions:

* Does it change over time?
* Does it depend on other factors that can change?
* Can it be reconstructed or derived from other data?

5. A good rule of thumb is to try to keep state as close to the components that use it as possible. In other words, if a component needs to manage some state, that state should be stored in the component or in a parent component that manages the state for multiple child components. This helps to keep the application organized and makes it easier to reason about how data is flowing through the system.


## Ques for higher order function

1. A higher-order function is a function that takes one or more functions as arguments or returns a function as its result. In other words, it is a function that operates on functions. Higher-order functions are a powerful concept in functional programming because they allow us to write more reusable and composable code.
2. The greaterThan function is an example of a higher-order function. It takes a number as an argument and returns a new function that takes another number and returns true if that number is greater than the original number, and false otherwise.
Line 2 of the greaterThan function is defining a new function using a shorthand syntax called arrow functions. 
3. Map takes a function as its argument and applies that function to each element in an array, creating a new array with the results. Reduce takes a function as its argument and uses that function to accumulate a single value by iteratively combining each element of an array. 

## Things i want to know more about 

I want to learn more about higher order functions and getting more understanding using filter. 