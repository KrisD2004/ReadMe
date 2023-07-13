# Classes & Memory Management

## Introduction to classes

* Reference Types: Classes in C# are reference types. When you declare a variable of a reference type, it initially contains the value null until you create an instance of the class using the new operator.

* Declaring Classes: To declare a class, use the class keyword followed by a unique identifier. You can also specify an access modifier (e.g., public) to control the visibility of the class.

* Creating Objects: A class defines a type of object, but an object itself is a concrete instance based on a class. You can create objects by using the new keyword followed by the class name.

* Constructors and Initialization: When you create an instance of a class, you can initialize its fields and properties to useful values. Initialization can be done through default values, field initializers, constructor parameters, or object initializers.

* Class Inheritance: Classes in C# support inheritance. You can derive a class from another class (base class) to inherit its data and behavior. Inheritance is specified using a colon followed by the name of the base class.

* Abstract and Sealed Classes: An abstract class contains abstract methods without implementation and cannot be instantiated. It can only be used through derived classes that implement the abstract methods. A sealed class, on the other hand, doesn't allow other classes to derive from it.

* Interfaces: A class can implement one or more interfaces, which define a contract for the behavior that the class should provide. Interfaces enable polymorphism and multiple inheritance of behavior.

* Splitting Class Definitions: Class definitions can be split between different source files using partial classes and methods. This can be useful for organizing and managing large classes.

## Constructors (C# programming guide)

* Constructors: Whenever an instance of a class or struct is created, its constructor is called. A constructor is a special method with the same name as the class or struct. It is responsible for initializing the newly created object.

* Multiple Constructors: A class or struct can have multiple constructors, each with a different set of parameters. This allows for different ways to initialize objects of the class or struct. Constructors enable you to set default values, enforce certain initialization logic, and provide flexibility in object creation.

* Initialization Order: When a new instance is initialized, several actions take place in a specific order. First, instance fields are set to their default values. Then, field initializers are executed, followed by base type field initializers. Next, base instance constructors run, starting from the base class to the direct base class. Finally, the instance constructor for the current type runs.

* Constructor Syntax: The syntax for defining a constructor includes the optional access modifier, the constructor name (which is the same as the class or struct name), and the parameter list. Constructors don't have a return type. They are used to initialize the object's state based on the provided arguments.

* Expression Body Definition: If a constructor can be implemented as a single statement, you can use an expression body definition. It provides a more concise way to define the constructor using the lambda-like syntax.

* Static Constructors: In addition to instance constructors, a class or struct can have a static constructor. Static constructors are used to initialize static members of the type. They are parameterless and are automatically called before any static member is accessed or any instance of the class or struct is created.

## Properties (C# Programming Guide)

* Properties Overview: Properties provide a flexible mechanism to read, write, or compute the value of a private field. They can be used as if they were public data members but are special methods called accessors. Properties allow for controlled access to data and promote safety and flexibility in methods.

* Get and Set Accessors: Properties have get and set accessors. The get accessor returns the property value, and the set accessor assigns a new value. In C# 9 and later, an init accessor can be used to assign a value only during object construction.

* Read-Write, Read-Only, and Write-Only Properties: Properties can be read-write (both get and set accessors), read-only (only get accessor), or write-only (only set accessor). Write-only properties are rare and used to restrict access to sensitive data.

* Properties with Backing Fields: One common pattern for implementing a property involves using a private backing field to store the value. The get accessor returns the value of the field, and the set accessor performs validation or conversions before assigning a new value to the field.

* Expression Body Definitions: Property accessors can be implemented as expression-bodied members, which provide a concise syntax for simple getter or setter logic. Expression body definitions use the => symbol followed by the expression to assign or retrieve the property value.

* Auto-implemented Properties: In cases where the property logic is simple, auto-implemented properties can be used. Auto-implemented properties allow the compiler to automatically generate the backing field and implement the get and set accessors.

* Required Properties: Starting from C# 11, the required keyword can be used to mark properties as required, forcing client code to initialize those properties. This helps ensure that the necessary data is provided during object initialization.

Remember, properties provide a way to encapsulate data and control access to it. They offer more control and flexibility compared to directly exposing fields as public members. If you have any specific questions or need further clarification on any of these topics, feel free to ask!

### Properties Questions

1. What’s the difference between a static and an instance constructor?

* Static constructors are parameterless. A static constructor is a constructor declared using static modifier. It is the first block of code executed in a class. With that, a static constructor executes only once in the life cycle of class. Instance constructor initializes instance data. Instance constructor is called when an object of class is created.

2. How does the use of a static constructor differ from setting properties/values?

A static constructor initializes static fields or properties of a class only once when the class is loaded into memory. This differs from setting properties or values, which is done for each instance of the class separately. Static constructors cannot be called explicitly, while setting properties or values can be done at any time.

## stack and heap

The Stack is more or less responsible for keeping track of what's executing in our code (or what's been "called").  The Heap is more or less responsible for keeping track of our objects(our data..well most of it).

4 main types of things we going to be put in the Stack and heap are: Value Types, Reference Types, Pointers, and Instructions.

In C#, all the "things" declared with the following list of type declarations are Value types

* Value Types: bool, byte, char, decimal, double, enum, float, int, long,sbyte, short, struct, uint, ulong, ushort

All the "things" declared with the types in this list are Reference types (and inherit from System.Object... except, of course, for object which is the System.Object object)

* Reference types: class, interface, delegate, object, string

### Questions stack and heap

1. Knowing about the stack and the heap, I might consider the following strategies to make more efficient use of memory in my projects:

Avoid creating too many unnecessary objects that are stored on the heap. I would try to reuse objects whenever possible rather than creating new ones. Consider using value types instead of reference types where appropriate. Value types are stored on the stack and are more efficient in terms of memory usage.

## Fundamentals of garbage collection

* Garbage collector provides the following benenfits:
-Frees developers from having to manually release memory.
-Allocates objects on the managed heap efficiently.
-Reclaims objects that are no longer being used, clears their memory, and keeps the memory available for future allocations. Managed objects automatically get clean content to start with, so their constructors don't have to initialize every data field.
-Provides memory safety by making sure that an object can't use for itself the memory allocated for another object.

### Questions on Garbage collection

1. Compare “Garbage Collection” in C# with the lifecycle of normal household items.

Garbage collection in C# to the lifecycle of household items, stating that both involve managing and disposing of unwanted or unneeded items. Garbage collection involves the automatic removal of unused objects from memory, improving performance. Similarly, household items are acquired, used, and eventually disposed of in a responsible manner. Both garbage collection and households need periodic management to ensure optimal performance and a clean, organized living space.

## Things i want to know more about 
