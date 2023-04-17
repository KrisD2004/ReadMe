# Introduction to React and Components

Component and React

## Component-Based Architecture

* Component-based architecture focuses on the decomposition of the design into individual functional or logical components that represent well-defined communication interfaces containing methods, events, and properties.

* The primary objective of component-based architecture is to ensure component reusability.

* A component encapsulates functionality and behaviors of a software element into a reusable and self-deployable binary unit. There are many standard component frameworks such as COM/DCOM, JavaBean, EJB, CORBA, .NET, web services, and grid services.

## Component

A software component is a modular and portable piece of software that encapsulates well-defined functionality and is intended to interact with other components. It has a clearly defined interface and conforms to a recommended behavior. It can be deployed independently and is subject to composition by third parties.

A component can have 3 different views - object-oriented view, conventional view, and process-related view.

* The object-oriented view considers a group of classes that work together to solve a problem. The analysis identifies problem domain classes, and the design identifies infrastructure classes, each with their own attributes and operations. The interfaces between classes are also defined to enable communication and cooperation.

* The conventional view sees a program module as a functional element that contains processing logic, internal data structures, and an interface for invoking the component and passing data to it.

* The process-related view involves building a system using existing components from a library, rather than creating each component from scratch. The software architecture is created, and components are selected from the library and integrated into the architecture.

## Characteristics of Components

Reusability, replaceable, not context specific, extensible, escapsulated, and independent are all characteristics of components

* Reusability − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.
* Replaceable − Components may be freely substituted with other similar components.
* Not context specific − Components are designed to operate in different environments and contexts.
* Extensible − A component can be extended from existing components to provide new behavior.
* Encapsulated − A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.
* Independent − Components are designed to have minimal dependencies on other components.

## Principles of Component−Based Design

* The software system is decomposed into reusable, cohesive, and encapsulated component units.
* Each component has its own interface that specifies required ports and provided ports; each component hides its detailed implementation.
* A component should be extended without the need to make internal code or design modifications to the existing parts of the component.
* Depend on abstractions component do not depend on other concrete components, which increase difficulty in expendability. 
* Connectors connected components, specifying and ruling the interaction among components. The interaction type is specified by the interfaces of the components.
* Components interaction can take the form of method invocations, asynchronous invocations, broadcasting, message driven interactions, data stream communications, and other protocol specific interactions.
* A component can extend to other components and still offer its own extension points. It is the concept of plug-in based architecture. This allows a plugin to offer another plugin API.

## Conducting Component-Level Design

The advantages of using component-based design include ease of deployment, reduced cost, reusability, reliability, and system maintenance and evolution. Component-based design allows for independent development of components and flexible connectivity between them.

# Props and how to use it in React

React is a library that follows a component-based approach to UI development, where the UI is divided into reusable components. In some cases, these components need to communicate with each other by passing data. To achieve this, React uses "props" or properties, which are a way to pass data from a parent component to a child component. 

**Prop** is a keyword in react which means properties and is being used for passing data from one component to another. 
Props flows from top to bottom(Parent to Child).

## Questions

Component 

1. A component is a modular and reusable piece of code that encapsulates a set of functionality and renders a part of the UI.
2. Reusability, replaceable, not context specific, extensible, escapsulated, and independent are all characteristics of components
3. The advantages of component based architecture are reusability, maintenance, collaboration, and consistency. 

Prop Questions
1. Prop is short of properties
2. In React, props (short for "properties") are used to pass data from a parent component to a child component.
3. parent to child is the flow(top to bottom)


## Things i want to know more about

* I want to know more about props 