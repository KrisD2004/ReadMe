# React and Forms

## Forms

* In React, form elements are treated as "controlled components". This means that the state of the form is controlled by React, not the DOM.
* To create a controlled component, you need to add an event handler for the input's onChange event. This event handler should update the component's state with the new value of the input.
* You can then use the component's state to set the value of the input. This means that the input's value will always reflect the current state of the component.
* You can also use the component's state to control other aspects of the form, such as the disabled state of a button or the selected value of a dropdown.
* In React, you can use the onSubmit event of a form to handle form submission. To prevent the default form submission behavior, you should call event.preventDefault() in your event handler.
* You can use the value prop to set the default value of an input. This can be useful when you want to reset the form to a default state.
* You can use the defaultValue prop to set the initial value of an input that can be changed by the user.
* In React, you can use the ref attribute to get a reference to a DOM node. This can be useful when you need to interact with the DOM directly, such as when you need to focus an input field.
* In some cases, you may want to use uncontrolled components instead of controlled components. Uncontrolled components rely on the DOM to store the form state, rather than using React's state. This can be useful for simple forms where you don't need to track every change to the form.
* In React, you can use third-party libraries to handle form validation. Some popular options include Formik, React Hook Form, and Yup.

## JavaScript: The Conditional (Ternary) Operator

* The ternary operator is a shorthand way of writing conditional statements in JavaScript.
* It consists of three parts: a condition, a question mark (?), and two expressions separated by a colon (:).
* If the condition evaluates to true, the first expression is executed; if it evaluates to false, the second expression is executed.
* The ternary operator is often used as a shortcut for simple if-else statements.
* It can also be nested inside other ternary operators to create more complex conditional expressions.
* One important thing to note is that the ternary operator can make code more difficult to read and understand, especially if it is used excessively or inappropriately.
* It is best used for simple, one-line conditional statements where the code is still easy to follow.
* The article provides several examples of how to use the ternary operator in different contexts, such as setting default values or checking for null or undefined values.
* Finally, the article concludes with some tips on when to use and when to avoid the ternary operator in JavaScript code. 

## Forms Questions

1. A 'controlled component' in React refers to an input form element whose value is controlled by React through its state. This means that the value of the form element is kept in the component's state and is updated whenever the user types in the input field.
2. In most cases, it's better to update the state with the user's responses as soon as they enter them, rather than waiting until they submit the form. There are several reasons for this:

Real-time feedback: Updating the state with the user's responses as they enter them allows for real-time feedback and validation. This means that the user can see the results of their input immediately, rather than having to wait until they submit the form to see if there are any errors.

Improved user experience: By providing real-time feedback, users are more likely to have a positive experience with the form. They can see what they are doing correctly and what they need to fix in real-time, which can be very helpful.

Easier to manage: Storing the user's responses in state as they enter them can also make it easier to manage the data. When the user submits the form, you can simply grab the data from state and process it, rather than having to collect all of the data from the form fields.

That being said, there may be some cases where you want to wait until the user submits the form to update the state. For example, if you have a multi-page form, it may be better to update the state only after the user has completed all the pages and submitted the form. However, in most cases, updating the state with the user's responses as they enter them is the better approach.
3. To target what the user is entering if we have an event handler on an input field, we can use the **event.target.value property** to get the current value of the input field.

## ternary 

1. The ternary operator is used as a shorthand for an if...else statement when there are only two possible outcomes.
2. console.log(x === y ? true : false);

