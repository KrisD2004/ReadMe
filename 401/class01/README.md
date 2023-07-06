# Exception Handling

## Lab 1a Reading Material (Numbers Game)

1. Prerequisites:

* Make sure you have Visual Studio Code installed and the C# extension added. You can install extensions in Visual Studio Code by navigating to the VS Code Extension Marketplace.
* Install the .NET 7 SDK on your machine. You can download it from the official .NET website.

2. Creating the app:

* Open Visual Studio Code and select "File > Open Folder" from the main menu.
* Create a new folder named "HelloWorld" and select it.
* Trust the authors of the files in the folder when prompted.
* Open the Terminal in Visual Studio Code by selecting "View > Terminal" from the main menu.
* In the Terminal, run the command dotnet new console --framework net7.0 to create a new .NET console app project.

3. Modifying the code:

* Replace the contents of the Program.cs file with the provided code in the tutorial. This code sets up a simple console application that prints "Hello, World!" to the console.
* If Visual Studio Code doesn't prompt you to add the missing assets for building and debugging, you can manually create the launch.json and tasks.json files by selecting "Run > Add Configuration" from the menu and choosing the appropriate options.

4. Running the app:

* Use the command dotnet run in the Terminal to run the application.
* The program will display "Hello, World!" in the console.

5. Enhancing the app:

* Modify the code in the Main method of Program.cs to prompt the user for their name and display it along with the current date and time.
* Save your changes in Visual Studio Code before running the program again.

## User Input & Conversion

* Console.ReadLine(): This method is used in C# to read a line of input from the user via the console. It returns the input as a string.

* Getting User Input: To get user input, you can use Console.ReadLine() and store the input in a variable of type string.

* Converting to Other Data Types: If you need to convert the user input to a different data type, such as int or double, you can use the Convert.ToX methods, where X represents the desired data type. For example, Convert.ToInt32() converts a string to an integer.

* Type Casting: Type casting is the process of converting a value from one data type to another. It can be done explicitly using the appropriate casting syntax, such as (int) or by using the Convert.ToX methods.

* Error: When you try to assign a string value obtained from Console.ReadLine() directly to an int variable, it will cause an error because you cannot implicitly convert a string to an int.

* Handling the Error: To convert a string to an int, you need to use the Convert.ToInt32() method explicitly to perform the conversion and store the result in an int variable.

* Printing Output: You can use Console.WriteLine() to print values to the console. You can concatenate strings with variables using the + operator.

## C# Methods

* Methods: Methods in C# are blocks of code that perform specific actions or tasks. They are defined with a name, optional parameters, and a body that contains the code to be executed.

* Method Signature: The method signature consists of the method's name and its parameter list (if any). It helps identify and differentiate methods.

* Method Declaration: To declare a method, you specify the access modifier (e.g., static), return type (e.g., void), method name, and any parameters within parentheses.

* Access Modifiers: Access modifiers (e.g., public, private) define the visibility and accessibility of methods. They determine whether the method can be accessed by other parts of the program.

* Parameters: Parameters are optional and allow you to pass data to a method. They are defined within the parentheses after the method name. A method can have multiple parameters, separated by commas.

* Method Body: The method body contains the code to be executed when the method is called. It is enclosed in curly braces ({ }).

* Calling a Method: To execute (call) a method, you write its name followed by parentheses and a semicolon. This triggers the execution of the code within the method.

* Reusability: Methods are used to encapsulate a specific set of actions, allowing you to reuse code throughout your program. By defining a method once, you can call it multiple times from different parts of your program.

* Main Method: The Main method serves as the entry point of a C# program. It is automatically executed when the program starts.

* Method Naming Convention: In C#, it's common to use PascalCase (starting with an uppercase letter) for method names to follow naming conventions and enhance code readability.

## Notes on Debugging C# Code using Visual Studio

* The Visual Studio debugger provides various features to help debug and analyze code while it's running.
* Debugging allows you to step through code, inspect variables, set breakpoints, and examine the call stack.
* Before starting to debug, ensure that Visual Studio 2019 is installed with the .NET Core cross-platform development workload.
* To create a project, open Visual Studio, go to File > Start Window, and choose "Create a new project".
* Search for "console" in the project templates, select the "Console Application" template for .NET Core, and enter a project name.
* After creating the project, open the Program.cs file and replace the default code with the provided code.
* The code creates a simple console application that uses arrays, loops, and a custom method.
* To start debugging, press F5 or click the "Start Debugging" button in the Debug Toolbar.
* Set breakpoints in the code by clicking in the left margin of a line, which will suspend the execution at that point.
* When the debugger hits a breakpoint, you can inspect variables by hovering over them or expanding their properties.
* Use F10 (or Debug > Step Over) to execute the current line and move to the next line.
* F11 (or Debug > Step Into) allows you to step into method calls and examine their execution.
* Shift + F11 (or Debug > Step Out) lets you quickly return from a method and continue debugging.
* The call stack shows the sequence of method calls that led to the current point in the code.
* You can continue debugging by pressing F5 (or Debug > Continue) to resume normal execution until the next breakpoint or the end of the program.

## How to debug for absolute beginners

* Clarify the Problem:
Identify what you expected your code to do and what actually happened.
If there's an error or exception, pay attention to the error message and try to understand its meaning.
Challenge your assumptions about the code and its behavior.

* Examine Your Assumptions:
Verify if you're using the correct API, function, method, or property.
Check if you're using an API correctly or if you made any typos.
Question any changes you made to the code and their potential impact.
Ensure your variables contain the expected values.
Understand the intent of the code, especially if it's not your own.

* Step through Your Code in Debugging Mode:
Use a debugging tool like Visual Studio to run your code step by step and monitor its execution.
Enter debugging mode by pressing F5 or using the "Start Debugging" button in Visual Studio.
Set breakpoints at specific lines of code to pause the execution and examine the program state.
Use the debugger's features to inspect variables, memory, and the sequence of code execution.
Pay attention to exceptions or errors and let the debugger guide you to the relevant code.

* Summary:
Debugging helps identify and fix programming mistakes by running code in a step-by-step manner.
It's essential to clarify the problem, question assumptions, and use debugging tools effectively.
Asking the right questions, examining code assumptions, and stepping through code are key steps.

* Next Steps:
Continue practicing and gaining experience with debugging tools and techniques.
Learn about additional debugging features and best practices.
Collaborate with experienced developers to learn from their debugging strategies.


Debugging is a valuable skill for software developers, and with practice, you can effectively identify and resolve issues in your code. Remember to approach debugging systematically, ask the right questions, and make use of available debugging tools to make your debugging process more efficient.


### Things i want to know more about  