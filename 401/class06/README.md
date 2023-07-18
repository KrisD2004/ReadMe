# Object Oriented Principles

## Inheritance - derive types to create more specialized behavior

* Inheritance: The article explains that inheritance allows you to create new classes that reuse, extend, and modify the behavior defined in other classes. It mentions that a derived class can have only one direct base class but can inherit members from multiple levels of inheritance.

* Abstract and virtual methods: The article describes how virtual methods can be overridden by derived classes, providing their own implementation. It also explains that abstract methods must be overridden in non-abstract classes that directly inherit from the abstract class. Abstract and virtual methods enable polymorphism.

* Abstract base classes: The article introduces abstract classes, which cannot be instantiated directly but can be used as a base for derived classes. Abstract classes can contain abstract methods that must be implemented by derived classes. It mentions that derived classes that are not abstract must provide implementations for abstract methods.

* Interfaces: The article explains that interfaces define a set of members that must be implemented by classes or structs that implement the interface. It mentions that a class can implement multiple interfaces but can only derive from a single direct base class.

* Preventing further derivation: The article mentions that a class or member can be marked as sealed to prevent other classes from inheriting from it. Sealed classes cannot be used as base classes.

* Derived class hiding of base class members: The article explains that a derived class can hide base class members by declaring members with the same name and signature. It introduces the new modifier, which can be used to explicitly indicate that the member is not intended to be an override of the base member.

## Abstract and Sealed Classes and Class Members

1. Abstract Classes and Class Members:

* An abstract class is declared using the abstract keyword before the class definition.
* An abstract class cannot be instantiated and is meant to serve as a base class for derived classes.
* Abstract classes can define abstract methods, which are declared using the abstract keyword and have no implementation.
* Derived classes of an abstract class must implement all the abstract methods.
* Abstract classes can override virtual methods from a base class with abstract methods.

1. Sealed Classes and Class Members:

* A sealed class is declared using the sealed keyword before the class definition.
* A sealed class cannot be used as a base class and cannot be an abstract class.
* Sealed classes prevent further derivation, and they can provide certain runtime optimizations.
* In a derived class, a method, indexer, property, or event that overrides a virtual member of the base class can be declared as sealed to prevent further overriding.
* It's worth noting that abstract classes are used when you want to define a common base class with shared behavior, whereas sealed classes are used to prevent further derivation and restrict the class from being used as a base.

## Polymorphism

Polymorphism:
Polymorphism is the third pillar of object-oriented programming, alongside encapsulation and inheritance.
It refers to the ability of objects of different derived classes to be treated as objects of a common base class.
Polymorphism allows for flexibility and extensibility in code by enabling interaction with objects at a higher level of abstraction.

Runtime Polymorphism:
At runtime, objects of a derived class can be treated as objects of a base class.
This allows for substitutability, as the object's declared type doesn't have to be identical to its runtime type.
Polymorphism at runtime is useful for method parameters, collections, arrays, and more.

Virtual Methods:
Base classes can define virtual methods, which can be overridden by derived classes.
Virtual methods have their implementation determined at runtime based on the actual type of the object.
This enables derived classes to provide their own implementation while still adhering to the base class's contract.

Polymorphism in Practice:
To demonstrate polymorphism, the article provides an example of a drawing application with different shape classes.
A base class called Shape is created with a virtual method Draw().
Derived classes such as Circle, Rectangle, and Triangle override the Draw() method with their specific implementations.
A list of Shape objects is created, containing instances of different shape classes.
By calling the Draw() method on each shape object, the appropriate overridden implementation is invoked, demonstrating polymorphic behavior.

Virtual Members and Overrides:
Virtual members in base classes allow derived classes to define new behavior by overriding them.
Derived classes can inherit the closest base class method without overriding it, preserving the existing behavior.
Derived classes can also define new non-virtual implementations that hide the base class implementations.
The override keyword is used to indicate that a method is intended to participate in virtual invocation.

Hiding Base Class Members:
If a derived class wants to have a member with the same name as a member in the base class, the new keyword can be used to hide the base class member.
Hidden base class members can still be accessed by casting the derived class instance to the base class type.

Preventing Overriding of Virtual Members:
Virtual members can be overridden by derived classes unless the sealed keyword is used to prevent further inheritance.
Declaring an override as sealed stops virtual inheritance, and the method is no longer virtual to any class derived from the sealed class.

Accessing Base Class Virtual Members from Derived Classes:
A derived class that has overridden a method or property can still access the base class implementation using the base keyword.
This allows the derived class to extend the base class's behavior while still utilizing the base class's implementation.

## Object-Oriented programming (C#)

* C# is an object-oriented programming language that follows four basic principles: Abstraction, Encapsulation, Inheritance, and Polymorphism.
* Abstraction involves modeling relevant attributes and interactions of entities as classes to define an abstract representation of a system.
* Encapsulation involves hiding the internal state and functionality of an object and only allowing access through a public set of functions.
* Inheritance allows creating new abstractions based on existing abstractions.
* Polymorphism enables implementing inherited properties or methods in different ways across multiple abstractions.
* The article discusses extending an application to create different types of accounts by using inheritance and polymorphism.
* New account types (InterestEarningAccount, LineOfCreditAccount, GiftCardAccount) are created as derived classes that inherit methods and data from the base BankAccount class.
* The derived classes override a virtual method called PerformMonthEndTransactions to add specific functionality for each account type.
* The article also covers additional modifications to the BankAccount class to handle minimum balance, overdraft rules, and fees for LineOfCreditAccount.
* The code examples provided demonstrate the usage of the different account types and their functionalities.


## Things i want to know