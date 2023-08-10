# Dependency Injection & Repository Design Pattern

## Design the infrastructure persistence layer

This article discusses the design of the infrastructure persistence layer in .NET microservices architecture. It introduces the Repository pattern, which separates data access from the domain model, and explains its benefits, such as better maintainability and decoupling. The article emphasizes defining one repository per aggregate and enforcing one aggregate root per repository. It also introduces the Unit of Work pattern, which handles multiple database operations in a single transaction. The article suggests implementing repositories as needed, as they are not mandatory in DDD design. It provides additional resources for further understanding of the Repository and Unit of Work patterns.

Key points:

* Repository pattern separates persistence concerns from the domain model.
* Each aggregate should have a corresponding repository class.
* Repositories control transactional consistency for aggregates.
* Unit of Work pattern handles multiple operations in a single transaction.
* Implement repositories based on your project's needs.

## 30 Days of TDD: Day Five – Make Your Code SOLID


This blog post discusses the SOLID principles of software development and their relevance to Test-Driven Development (TDD). It introduces the 
five SOLID principles:

Single Responsibility Principle (SRP): Each method or class should have only one responsibility. This principle promotes focused and maintainable code.

Open/Closed Principle (OCP): Software entities should be open for extension but closed for modification. This principle encourages creating flexible and extensible designs.

Liskov Substitution Principle (LSP): Objects of derived classes should be substitutable for objects of the base class without affecting the correctness of the program. This principle ensures compatibility and consistency in inheritance hierarchies.

Interface Segregation Principle (ISP): Clients should not be forced to depend on interfaces they do not use. This principle encourages creating specific and targeted interfaces to avoid unnecessary dependencies.

Dependency Inversion Principle (DIP): High-level modules should not depend on low-level modules. Both should depend on abstractions. This principle promotes loose coupling and flexibility in software design.

The author explains each principle and how they contribute to writing better software. The post emphasizes the benefits of adhering to these principles, such as easier testing, maintainability, and extensibility. The concepts are related to Test-Driven Development (TDD), which is a development process where tests are written before the actual code. The SOLID principles align with TDD by encouraging modular, testable, and flexible code designs.

The author also mentions that adhering to these principles can be particularly beneficial when combined with tools like JustCode and JustMock, which assist in practicing TDD.

## Things i want to know 