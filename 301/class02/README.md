# State and Props

## React: Component Lifecycle Events

Component lifecycle events in React refers to the series of stages that a component goes through from initialization to destruction. **Mounting**, **Updating**, and **Unmounting** are the 3 phases of the component lifecycle. 

* Mounting is when an instance of a component is being created and inserted into the DOM and it occurs during the mounting phase. Constructor,static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.

* Updating is anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.
static getDerivedStateFromProps, shouldComponentUpdate, render,
getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps

* Unmounting is the last phase of the cycle and its called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase. 

## Questions for React lifecycle

1. The render happens before the componentDidMount.
2. Mounting is the first thing to happen in the lifecycle. 
3. Constructor - render - react updates- componentdidmount- componentWillUnmount. This is the correct order. 
4. ComponentDidMount is a method that is invoked immediately after a component is mounted. 


## React state vs Props

This video talks about the differences between props and states. 

States is a way for components to store and manage data that can change over time. 

Props on the other hand are a way for components to recieve data from their parent components.

## Questions for React State v Props

1. You can pass strings, numbers, booleans, objects, functions, arrays and react elements.
2. The difference is state store and manage data that can be changed over time while props **recieve data from the parent components**
3. React will re-render the component to update the UI.
4. You can store form input values, user authentication state, and Component visibility.