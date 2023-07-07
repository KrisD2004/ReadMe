# Unit Testing and Documentation

## Unit testing 

* What Unit Testing Isn't:
Unit tests don't deal with the environment or external systems.
They are not smoke tests, load tests, or end-to-end system tests.

* What Unit Testing Is:
Unit tests isolate and exercise specific units of code.
In C#, a unit can be a method, and a unit test tests a specific aspect of that method in isolation.

* Unit Testing Tutorial:
A simple example is given using a Calculator class with an Add method.
A clunky unit test is demonstrated by running the code in a console project.
The need for a unit test framework is introduced to make testing easier and more efficient.

* Introducing a Unit Test Framework:
The article suggests using a unit test project template and a test framework (such as MSTest in this case).
A sample unit test is provided using the framework, demonstrating the use of the Assert class to validate the test results.

* Anatomy of a Unit Test:
The test class is given a descriptive name (e.g., CalculatorTests).
Test methods are named to describe the hypothesis being tested (e.g., Adding_4_And_3_Should_Return_7).
The TestClass and TestMethod attributes are used to mark the test class and methods.
The Assert class is used to perform assertions and determine the success or failure of the test.

* Importance of Unit Testing:
Unit testing helps catch bugs early in the development cycle.
It improves code quality and prevents errors and unexpected behavior.
It allows for more frequent releases and encourages good programming habits.

* Unit Testing Best Practices:
Arrange, Act, Assert: Follow the logical components of a good unit test.

Use relevant and high-quality test data.

Aim for one assert per test method to improve test clarity.

Avoid test interdependence to ensure independence and reliability.

Consider writing tests before writing code (Test Driven Development).

Keep test setup short, sweet, and visible for easy understanding.

Use headless testing when appropriate for efficiency and consistency.

Test positive and negative scenarios, including boundary conditions.

Use mock objects to simulate dependencies and isolate code being tested.

Ensure compliance with industry standards and document compliance testing.

Ensure tests are repeatable and deterministic.

Test for security vulnerabilities to ensure application security.

Recognize test setup pain as a design problem and improve code modularity.

Add unit tests to the build process to ensure their execution and reliability.


## Using .NET Core with Visual Studio

* To create a unit test project using xUnit.net, start Visual Studio and click "Create a new project" from the start splash screen.
* In the new project wizard, select the language (C#), platform (All platforms), and project type (Test). Choose "xUnit Test Project (.NET Core)" from the available project templates and click "Next".
* Provide a name for the project and click "Create". Visual Studio will launch with the newly created project.
* The project file (csproj) includes references to the required packages for xUnit.net and test execution. You can modify the target framework and remove redundant lines if necessary.
* Test Explorer is a window in Visual Studio that allows you to browse and run your tests. Open Test Explorer by selecting "Test > Test Explorer" from the main menu.
* Test Explorer displays a tree view of the tests in your project and provides buttons for running tests, filtering the test list, and configuring options.
* You can run all tests in the Test Explorer by clicking the "Run All Tests In View" button. Test results will be displayed, indicating whether the tests passed or failed.
* To write tests, edit the default UnitTest1.cs file and replace the default code with your own test methods.
* xUnit.net supports two types of tests: facts and theories. Facts are tests that are always true, while theories are tests that are only true for specific data sets.
* Facts are defined using the [Fact] attribute, while theories use the [Theory] attribute. You can provide test data for theories using the [InlineData] attribute.
* After writing tests, run them again using Test Explorer to see the results. Failed tests will display the failure message and the exact line where the failure occurred.
* To run tests against multiple target frameworks, modify the project file by changing TargetFramework to TargetFrameworks and specifying the target frameworks you want to support.
* Test Explorer will display the test project multiple times, once for each target framework. You can run tests individually for each framework or run all tests for all frameworks.

## things i want to know more

