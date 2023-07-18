# Interfaces

* An interface is a construct in C# that defines a group of related functionalities that a class or struct must implement.
* Interfaces can include method signatures, properties, events, and indexers, but they cannot contain instance data such as fields or auto-implemented properties.
* Interfaces can define static methods that must be implemented and may provide default implementations for members.
* C# doesn't support multiple inheritance of classes, so interfaces are used to include behavior from multiple sources in a class.
* Structs in C# cannot inherit from other structs or classes, but they can implement interfaces to simulate inheritance.
* Interface names should start with a capital 'I' by convention.
* A class or struct that implements an interface must provide an implementation for all declared members of the interface.
* An interface can inherit from one or more interfaces, and a class implementing a derived interface must implement all members from both the derived interface and its base interfaces.
* Interfaces can be implicitly converted to their derived interfaces or any of their base interfaces.
* A class can include an interface multiple times through base classes or other interfaces, but it can provide an implementation of an interface only once.
* Interfaces can declare static members, and a class implementing the interface can also declare static members with the same signature without overriding the interface's static members.
* Properties and indexers of a class can have extra accessors compared to those defined in an interface, but explicit interface implementation requires matching accessors.
* A base class can implement interface members using virtual members, and a derived class can override those members to change the interface behavior.
* Interface members are public by default, but accessibility modifiers can be explicitly specified.
* Interface members cannot be instance fields, instance constructors, or finalizers.
* Interface members that aren't fields may be static abstract starting from C# 11.
* An interface cannot be instantiated directly; its members are implemented by classes or structs that implement the interface.
* In earlier C# versions, interfaces were like abstract base classes with only abstract members, but starting from C# 8.0, interfaces can have default implementations for some or all of their members.

## What is an Interface?

* Interfaces aim to separate how something is used from how it is implemented.
* The main problem interfaces solve is allowing code to work with different implementations of a set of responsibilities without explicitly handling each implementation.
* Interfaces act as contracts, specifying that a class meets certain expectations and supports all the methods defined in the interface.
* Implementing an interface does not mean that the class is the interface itself; it means the class fulfills the contract defined by the interface.
* Interfaces should be designed to solve a specific problem or fulfill a particular contract, rather than describing the entire functionality of a class.
* Interfaces are usually implemented by more than one class, as they are meant to allow interaction with objects based on what they do, not how they do it.
* It's important to avoid creating unnecessary interfaces when the functionality is specific to a single class and doesn't require interaction with other classes.
* The YAGNI (You Ain't Gonna Need It) principle suggests not implementing an interface until there is a real need for it.
* Interfaces are not meant to be created solely for testing or dependency injection purposes; their purpose is to define contracts and enable polymorphism.
* Dependency injection can lead to interface abuse when interfaces are created solely for injecting the only implementation, adding unnecessary levels of indirection.
* Unit testing and dependency injection should focus on reducing dependencies and splitting classes rather than relying solely on interfaces for injection.
* The challenge lies in finding ways to unit test or use dependency injection without excessive interface creation, and exploring language-supported mechanisms for runtime implementation replacement.

## interface (C# Reference)

* An interface defines a contract that any implementing class or struct must adhere to by providing an implementation of the members defined in the interface.
* Interfaces can contain method signatures, properties, indexers, events, and default interface members.
* Default interface members provide a default implementation for classes or structs that don't provide their own implementation.
* Beginning with C# 11, interfaces can declare static abstract or static virtual members, typically used for defining overloaded operators or common functionality.
* Interface inheritance allows an interface to inherit from one or more base interfaces.
* When an interface overrides a method implemented in a base interface, it must use explicit interface implementation syntax.
* Interfaces can be implemented by multiple classes or structs.
* Interface members can be accessed through an instance of the interface, but not through a class instance that implements the interface.
* Interface inheritance syntax requires that the base class comes first in the base type list.
* Explicit interface implementation allows a class to implement interface members explicitly, making them accessible only through an instance of the interface.
* Interfaces can't contain instance fields or instance auto-properties, but they can include static fields and static constructor declarations.
* The C# language specification provides detailed information about interfaces, including default interface members and static abstract members.

### Things i want to know