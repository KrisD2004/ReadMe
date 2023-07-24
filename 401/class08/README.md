# Collections & Enums

## Collections in C #

### Introduction to Collections

* Collections in C# are used to group related objects.
* Arrays are useful for a fixed number of strongly typed objects, while collections provide more flexibility as they can grow and shrink dynamically.
* Arrays are useful for a fixed number of strongly typed objects, while collections provide more flexibility as they can grow and shrink dynamically.
* Collections can be created in two ways: using arrays of objects or using collections of objects.

### Using a Simple Collection

* The "List<T>" class is a generic collection that allows you to work with a strongly typed list of objects.
* You can use a collection initializer to initialize the collection with elements.
* Iteration through a collection can be done using foreach or for loops.
* Elements can be removed from the collection using the Remove() or RemoveAt() methods.

### Kinds of Collections

* Collections in C# are provided by different namespaces: System.Collections.Generic, System.Collections.Concurrent, and System.Collections.
* System.Collections.Generic classes are used for generic collections with strong typing, such as Dictionary<TKey, TValue> and List<T>.
* System.Collections.Concurrent classes provide efficient thread-safe operations for concurrent access.
* System.Collections classes store elements as object types and should be used when other collections are not suitable.

### Implementing a Collection of Key/Value Pairs

* The Dictionary<TKey, TValue> class allows access to elements in a collection using keys.
* The KeyValuePair<TKey, TValue> structure represents a key/value pair in the dictionary.
* You can use collection initializers to build dictionaries in a more concise way.
* You can retrieve elements from the dictionary using either ContainsKey(), Item[] property, or TryGetValue() method.

### Using LINQ to Access a Collection

* LINQ (Language-Integrated Query) can be used to access collections with filtering, ordering, and grouping capabilities.
* LINQ queries return a new collection with the desired results based on the query criteria.
* LINQ can be used with collections that implement IEnumerable<T> or IEnumerable.

### Sorting a Collection

* Custom sorting can be achieved by implementing the IComparable<T> interface and defining the CompareTo() method.
* The Sort() method can then be used to sort the collection based on the implemented comparison logic.
* You can also use LINQ to perform sorting and other operations on collections.

### Defining a Custom Collection

* Custom collections can be created by implementing the IEnumerable interface and providing a custom enumerator.
* Iterators can be used to perform custom iterations over a collection using the yield return statement.

### Iterators

* Iterators are used to perform custom iteration over a collection.
* Iterators can be implemented as methods or get accessors.
* The yield return statement is used to return each element of the collection one at a time during the iteration.

## Enumeration types 

* Enumeration Types: An enumeration type, or enum type, is a value type defined by a set of named constants of the underlying integral numeric type. Enums are defined using the enum keyword.

* Default Values: By default, the associated constant values of enum members are of type int and start with zero, increasing by one following the order of definition.

* Specifying Underlying Type and Values: You can explicitly specify any other integral numeric type as the underlying type of an enum. Additionally, you can specify custom constant values for enum members.

* Functionality: You cannot define a method inside the definition of an enumeration type. To add functionality, create an extension method.

* Representing Combination of Choices: To represent a combination of choices using enum, define enum members such that each choice corresponds to a bit field (powers of two). Use the bitwise logical operators | or & to combine or intersect choices. Apply the Flags attribute to indicate an enumeration type that declares bit fields.

* The System.Enum Type: System.Enum is the abstract base class of all enumeration types. It provides methods to get information about an enum type and its values.

* The Enum Constraint: You can use System.Enum in a base class constraint (enum constraint) to specify that a type parameter must be an enumeration type.

* Conversions: There are explicit conversions between an enumeration type and its underlying integral type. You can cast an enum value to its underlying type to get the associated integral value of an enum member. Boxing and unboxing conversions to and from System.Enum are also possible.

* Enum.IsDefined Method: Use this method to determine whether an enumeration type contains an enum member with a specific associated value.

* Examples: The article provides code examples to illustrate the usage of enum types, bit flags, enum constraint, and conversions.

Remember, enums are useful for representing sets of related constants and making the code more readable and maintainable. They are commonly used in scenarios where you have a fixed set of options to choose from. Additionally, using bit flags with enums allows for representing combinations of options, which is particularly useful in bit manipulation scenarios.

### Things i want to know more about 



