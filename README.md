## Week 1: 
## Day 1: 

### Intoduction to Java: 
What is Java?: 

Java is a class-based, object-oriented programming language that is designed to have as few implementation dependencies as possible. It is intended to let application developers write once, and run anywhere (WORA), meaning that compiled Java code can run on all platforms that support Java without the need for recompilation. 

#### JAVA COMPONENTS:

Theses are the required components for a Java program to function 

Java Code (.java): This is the code you write in the Java programming language. You save it in a file with a ".java" extension. 

Javac Compiler: This is a tool that takes your Java code and converts it into a special kind of code called "bytecode." The bytecode is saved in a file with a ".class" extension. 

Bytecode: It's a set of instructions that is not directly executed by the computer. Instead, it's an intermediate code that can be understood by the Java Virtual Machine (JVM). 

Java Virtual Machine (JVM): Think of it as a virtual computer inside your real computer. Its main job is to take the bytecode and execute it, making your Java program run. Each operating system has its own JVM, but they all produce the same results, making Java "platform-independent." 

Java Development Kit (JDK): This is a package that includes everything you need to develop Java programs. It contains the JRE (Java Runtime Environment), compilers (like javac), and various tools for debugging and documentation (JavaDoc). 

Java Runtime Environment (JRE): This is a subset of the JDK. It includes the JVM, which is necessary to run Java programs. If you only want to run Java programs and not develop them, you only need the JRE. 

In summary, as a Java programmer, you write code (.java), use the javac compiler to turn it into bytecode (.class), and then the JVM executes that bytecode. If you're developing, you use the JDK, and if you just want to run Java programs, you can use the JRE. 

 

#### MAIN JAVA FEATURES:

##### * Platform independent  
>>>What it means: Java programs can run on different types of computers without modification. 

>>>>Example: You write a Java program on a Windows computer, and it can run on a Mac or Linux computer without changes. 

##### * Object Oriented  
***What it means: Java is centered around the concept of "objects," which are instances of classes representing things or concepts in your program. 

***Example: If you're making a game, you might have objects like "Player" and "Enemy" with specific properties and behaviors. 

##### * Simple 
^^^^What it means: Java is designed to be easy to learn and use. 

^^^^Example: Java has straightforward syntax, making it accessible for beginners, and its automatic memory management (garbage collection) simplifies memory handling. 

##### * Robust Language 
>>What it means: Java is designed to be reliable and strong in handling errors and exceptions. 

>>Example: Java's strict compile-time checking helps catch errors before a program runs, reducing the chances of unexpected crashes. 

##### * Secure 
***What it means: Java provides features to create secure applications, protecting against various security threats. 

***Example: Java's "sandbox" security model ensures that untrusted code cannot harm the system it's running on. 

##### * Multithreading 
>>>>>What it means: Java supports the execution of multiple threads, allowing programs to perform multiple tasks concurrently. 

>>>>>Example: In a video player, one thread might handle user input, while another plays the video, providing a smoother user experience.

#### Typical Structure of a Java program:

##### *Package Declaration: 
A class in Java can be placed in different directories/packages based on the module they are used 
What: Think of it like putting your Java file in a labeled box. The label (package) helps organize classes. 
How: Use the package keyword to declare the package where your class belongs. 

##### *Import Statements: 

There can be classes written in other folders/packages of our working java project and also there are many classes written by individuals, companies, etc which can be useful in our program. To use them in a class, we need to import the class that we intend to use. Many classes can be imported in a single program and hence multiple import statements can be written. 
What: Imagine borrowing tools from different friends. Import statements let you use code (classes) from other "places" (packages). 
How: Use the import keyword to bring in classes from other packages. 

##### *Comments: 

The comments in Java can be used to provide information about the variable, method, class or any other statement. There are two ways to write comments in Java 
What: Leaving notes for yourself and others about your code. You can write short notes or longer explanations. 
How: Use // for short comments on one line and /* */ for longer comments covering multiple lines. 

##### *Class Definition: 
Naming your main group of code, like giving a title to a story. This is where your program's main structure begins. 
How: Use the class keyword followed by the class name. 

##### *Main Method: 
Execution of a Java application starts from the main method. In other words, it’s an entry point for the class or program that starts in Java Run-time. 
What: The starting point of your program. It's like the first instruction the computer reads when you run your program. 
How: Use public static void main(String[] args) – it's like a special set of instructions that gets executed first. 

##### *Methods/Behaviors: 
A set of instructions which form a purposeful functionality that can be required to run multiple times during the execution of a program. To not repeat the same set of instructions when the same functionality is required, the instructions are enclosed in a method.  
What: Imagine you have specific tasks to do. Methods are like mini-plans for those tasks, making it easy to repeat them. 
How: You create methods by enclosing sets of instructions. They can be called to perform their task when needed. 
So, in simple terms, a Java program is like a recipe: you organize your ingredients (code) in labeled boxes (packages), borrow tools (import statements) when needed, leave notes (comments) for yourself and others, give your recipe a title (class definition), start cooking from a specific point (main method), and have smaller plans (methods) for specific tasks. 
For now, just remember that every Java program has a class name which must match the filename, and that every program must contain the main() method. 

## Day 2: 
## Java Fundamentals: 
### WHAT IS A VARIABLE?:

Java variables=are containers for storing data values 
A variable is a name given to a memory location.  
The value stored in a variable can be changed during program execution. 
A variable is only a name given to a memory location; all the operations done on the variable effects that memory location. 
In Java, all the variables must be declared before use. 
In Java, there are different types of variables, for example 
String - stores text, such as "Hello". String values are surrounded by double quotes 
#### int:
stores integers (whole numbers), without decimals, such as 123 or -123 
#### float:
stores floating point numbers, with decimals, such as 19.99 or -19.99 
#### char: 
stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes 
#### boolean:
stores values with two states: true or false 

### Declaring (Creating) Variables: 
To create a variable, you must specify the type and assign it a value: 
Syntax  below 
type variableName = value;

Variables can be assigned values in two ways: 
* Variable Initialization 
* Assigning value by taking input 

### 3 TYPES OF VARIABLES IN JAVA: 

#### Local Variables: 
Definition: Variables defined within a block, method, or constructor. 
Scope: Exists only within the block where declared. Accessible only within that specific part of the code. 
Lifetime: Created when the block is entered or the function is called, destroyed when exiting the block or when the function call returns. 
Initialization: Mandatory. Must be given a value before use. 

#### Instance Variables: 
Definition: Non-static variables declared in a class, outside any method, constructor, or block. 
Scope: Exists throughout the entire class. Accessible from any method, constructor, or block within the class. 
Lifetime: Created when an object of the class is created, destroyed when the object is destroyed. 
Access: Can use access specifiers (public, private, etc.). Can be accessed only by creating objects of the class. 
Initialization: Not mandatory. Default value is 0. 
Number of Copies: Each object has its own copy of instance variables. 

#### Static Variables: 
Definition: Also known as Class variables. Declared with the static keyword within a class, outside any method, constructor, or block. 
Scope: Exists throughout the entire class. Accessible from any method, constructor, or block within the class. 
Lifetime: Created at the start of program execution, destroyed when program execution ends. 
Access: Accessed using the class name (e.g., ClassName.variable). Can also be accessed through object references but not recommended. 
Initialization: Not mandatory. Default value is 0. 
Number of Copies: Only one copy of a static variable exists per class, irrespective of how many objects are created. 

### Comparison: 

##### Instance Variable vs. Static Variable: 

###### Instance Variable: 
Each object has its own copy. Changes in one object don't affect others. 
###### Static Variable: 
Only one copy per class. Changes are reflected across all objects of the class. 

### Access: 
##### Instance Variable: 
Accessed through object references. 

##### Static Variable: 
Accessed using the class name. 
In summary, local variables are confined to a specific part of the code, instance variables belong to objects and have multiple copies, and static variables are shared among all objects of a class. 

### Data types in Java: 

Data type defines the values that a variable can take, for example if a variable has int data type, it can only take integer values.  
Java is a statically typed language; the data type of a variable is known at compile time. This means that you must specify the type of the variable (Declare the variable) before you can use it.  

##### In Java we have 2 categories of data type: 
###### 1. Primitive data types 
Primitive  data types include Booleans, char, byte, short, int, long, float and double.

##### Boolean:
The Boolean data type is used to store only two possible values: true and false. This data type is used for simple flags that track true/false conditions. 

##### Char:
The char data type is a single 16-bit Unicode character. Its value-range lies between '\u0000' (or 0) to '\uffff' (or 65,535 inclusive).The char data type is used to store characters. 

##### Byte:
It is an 8-bit signed two's complement integer.The byte data type is used to save memory in large arrays where the memory savings is most required. It saves space because a byte is 4 times smaller than an integer. It can also be used in place of "int" data type. 

##### Short:
The short data type is a 16-bit signed two's complement integer 
The short data type can also be used to save memory just like byte data type. A short data type is 2 times smaller than an integer. 

##### Int:
The int data type is a 32-bit signed two's complement integer.The int data type is generally used as a default data type for integral values unless if there is no problem about memory. 

##### Long:
The long data type is a 64-bit two's complement integer.The long data type is used when you need a range of values more than those provided by int. 

##### Float:
The float data type is a single-precision 32-bit IEEE 754 floating point.Its value range is unlimited.It is recommended to use a float (instead of double) if you need to save memory in large arrays of floating point numbers. The float data type should never be used for precise values, such as currency. Its default value is 0.0F. 

##### Double:
The double data type is a double-precision 64-bit IEEE 754 floating point. Its value range is unlimited. The double data type is generally used for decimal values just like float. The double data type also should never be used for precise values, such as currency. Its default value is 0.0d. 

###### 2. Non-primitive data types:
Classess,Arrays and Strings are non-primitive data types 

### Operators in Java: 
Operators are used to perform operations on variables and values. 
An operator is a character that represents an action, for example - is an arithmetic operator that represents subtraction. 
#### Java operators can be classified into: 
##### Arithmetic Operators:
this would be addition, subtraction, multiplication and division, increment and decrement. They are used to perform mathematical  operations 
##### Relational Operators:
these would be the equal, not equal,greater than, less than  
##### Bitwise Operators:
are used to performing the manipulation of individual bits of a number. They can be used with any integral type (char, short, int, etc.). 
##### Logical Operators:
Logical operators are used to determine the logic between variables or values. These would be logical AND, OR, NOT 
##### Assignment Operators:
used to assign a value to variables 
##### Misc Operators:
refers to various operators in Java that don't fall into the categories of arithmetic, relational, or logical operators.

### Java Classes and Objects:
In Java, a class is a fundamental concept that serves as a blueprint or template for creating objects. Objects, in turn, are instances of a class, and they have states (attributes) and behaviors (methods) 
Java is an object-oriented programming language. 
Everything in Java is associated with classes and objects, along with its attributes and methods.  
For example: in real life, a car is an object. The car has attributes, such as weight and color, and methods, such as drive and brake. 
* A Class is like an object constructor, or a "blueprint" for creating objects. 
* A class is a blueprint or template in Java that defines the behavior and state that the objects of its type will have. 
* It acts as a factory for creating objects. Without a class, you cannot create objects.
### Create a Class 
To create a class, use the keyword class.

### Constructors Explained: 
* A constructor is a special method that gets invoked when an object is created from a class. 
* It has the same name as the class and is responsible for initializing the object's state. 
* If you don't provide a constructor, Java automatically generates a default constructor. 
* Constructors can accept parameters, and a class can have more than one constructor.

### Create an Object:
* An object is an instance of a class. It represents a specific occurrence of that class in memory. 
* Objects have states (attributes/variables) and behaviors (methods). 
* In Java, an object is created from a class. We have already created the class named Main, so now we can use this to create objects. 
* To create an object of Main, specify the class name, followed by the object name, and use the keyword new.

### Methods: 
* Methods in a class represent the behavior or actions that objects of that class can perform. 
* They are defined within the class and can be called on objects of that class. 
* Methods can have parameters and return values. 

### Variables/Properties: 
* Variables or properties are attributes that describe the state of objects created from the class. 
* They are declared within the class and represent characteristics of objects. 

## Day 3: 
## Object Oriented Programming Concepts and Principles:
### What does OOP mean in Java?:
Object-oriented programming (OOP) is a computer programming model that organizes software design around data, or objects, rather than functions and logic. 
Object-oriented programming (OOP) is like organizing a toolbox. Instead of having various tools scattered around, we group related tools together in a single box, making it easier to find and use them.  
In OOP, a program is built around "objects" that combine data and actions (methods) in one place. This helps make programs more flexible and easier to maintain, like having a neatly organized toolbox. Java is a language that's good at this kind of organization. 
In OOP, computer programs are designed by making them out of objects that interact with one another 
Procedural programming is about writing procedures or methods that perform operations on the data, while object-oriented programming is about creating objects that contain both data and methods. 

### Object-oriented programming has several advantages over procedural programming: 
* OOP is faster and easier to execute 
* OOP provides a clear structure for the programs 
* OOP helps to keep the Java code DRY "Don't Repeat Yourself", and makes the code easier to maintain, modify and debug 
* OOP makes it possible to create full reusable applications with less code and shorter development time 

 

### Features of OOP – Core features:
#### 1.ABSTRACTION: 
Abstraction is a process of hiding the implementation details from the user, only the functionality will be provided to the user.  
In other words, the user will have the information on what the object does instead of how it does it. In Java, abstraction is achieved using Abstract classes and interfaces. 
Abstract classes and interfaces define what a thing does, but not how it does it. So, when you use a class or interface, you only need to know what it does, not the intricate details of its implementation. It's like using the TV remote without needing to understand the electronics inside – you just press the buttons to get the desired result. 
In programming, abstraction means hiding the complex inner workings of something and showing only what's necessary for the user. 

#### 2. ENCAPSULATION  
Encapsulation in Java is a mechanism of wrapping the data (variables) and code acting on the data (methods) together as a single unit.  
In encapsulation, the variables of a class will be hidden from other classes, and can be accessed only through the methods of their current class. Therefore, it is also known as data hiding. 
Encapsulation in Java is like packaging a gift. It's a way of bundling together the data (like a present inside a box) and the actions you can perform on that data (like unwrapping the gift) into a single unit.  
With encapsulation, you keep the details of how something works hidden from the outside, and only allow interaction through specific methods. 
##### * To achieve encapsulation in Java:
Declare the variables of a class as private. 
Provide public setter and getter methods to modify and view the variables values. 

#### 3.INHERITANCE 
Inheritance can be defined as the process where one class acquires the properties (methods and fields) of another. With the use of inheritance, the information is made manageable in a hierarchical order. 
Inheritance in programming is like passing on traits from one generation to another. It's a way for one class to acquire the characteristics (such as methods and fields) of another class. This process helps organize information in a structured and hierarchical manner. 
The class which inherits the properties of other is known as subclass (derived class, child class) and the class whose properties are inherited is known as superclass (base class, parent class). 
* 'extends' is the keyword used to inherit the properties of a class. In the example below class Sub inherits some of the properties from class Super. 

#### 4. POLYMORPHISM 
Polymorphism in programming is like a shape-shifting ability for methods. It allows you to process objects differently based on their data type.  
In simpler terms, it means having one method that can take different forms depending on the situation. 

##### Here's how polymorphism works: 
* Generic Interface: You design a generic interface that declares methods for a certain type of action. This interface serves as a common blueprint. 
* Multiple Implementations: Different classes can provide their own implementations of these generic methods. Each class may have its unique way of performing the specified action. 

###### Polymorphism can be implemented in 2 ways: 
* Overloading: This is like having multiple versions of the same method, each behaving differently based on the arguments passed. The decision on which version to use is made at compile time. 
* Overriding: This is when a subclass provides its own implementation for a method that is already defined in its superclass. The decision on which version of the method to use is made at runtime. 

### Other Features of OOP:

#### Coupling: 
* Definition: Coupling refers to the extent of dependency or knowledge that one class has about another class. Strong coupling occurs when one class is aware of the details of another class. 
#### Modifiers in Java: 
The visibility level of a class, method, or field is controlled using private, protected, and public modifiers. These modifiers help manage the visibility and access to the components of a class. 
* Weaker Coupling: Interfaces are used for weaker coupling because they provide a way to define a contract without specifying the concrete implementation. This reduces the dependency between classes. 

#### Cohesion: 
Definition: Cohesion measures how closely the methods in a class are related to each other and perform a single, well-defined task.                                                                                                                                                                                                                  while low cohesion means that a method performs multiple unrelated tasks. 

Example: The java.io package is highly cohesive because it contains classes and interfaces related to I/O operations. On the other hand, the java.util package is weakly cohesive as it encompasses unrelated classes and interfaces. 

#### Association: 
Definition: Association represents the relationship between objects. It can be one-to-one, one-to-many, many-to-one, or many-to-many. The relationship can be unidirectional or bidirectional. 

Examples: 
One country has one president (one-to-one). 
One president can have many cabinet ministers (one-to-many). 
Many cabinet ministers can have one prime minister (many-to-one). 
Many cabinet ministers can have many departments (many-to-many). 

#### Aggregation: 
Definition: Aggregation is a type of association that represents a one-way (HAS-A) relationship between two classes. It occurs when one class is dependent on another, but not vice versa. 
Example: Every Passenger has a Car, but a Car doesn't necessarily have a Passenger. 

 

#### Composition: 
Definition: Composition is a stricter form of aggregation where two classes are mutually dependent and can't exist without each other. 
Example: A Car and an Engine form a composition. A Car can't run without an Engine, and an Engine can't function without being part of a Car. 
In summary, these concepts are fundamental in object-oriented programming and help in designing classes and their relationships in a structured and effective manner. 

## Day 4: 
## Decision-Control: 
### Control Flow Statements: 
Definition: Control flow statements are used in programming to determine the order in which statements are executed. They allow the program to make decisions based on certain conditions and execute different sets of statements accordingly. 
Example Scenario: The example you provided involves making a decision based on a condition. For instance, you want to print "Positive Number" if a given number is greater than zero and "Negative Number" if it is less than zero. 
Purpose: Control flow statements help in directing the flow of the program, allowing it to adapt and make decisions dynamically during runtime. 

## Decision-Making Structures: 
Definition: Decision-making structures are a type of control flow statements that involve evaluating one or more conditions and executing specific statements based on whether these conditions are true or false. 
Example Explanation: 
Condition: The condition in your example is whether a number is greater than zero. 
Actions: If the condition is true, you want to execute the statement "Positive Number." If the condition is false, you want to execute the statement "Negative Number." 
Flexibility: These structures provide flexibility in programming by allowing the code to respond differently based on varying conditions during execution. 

## Conditional Statements in Java: 
In Java, the if statement is commonly used for decision-making. It evaluates a condition and, if true, executes a block of code. Optionally, an else block can be used to specify code that should be executed when the condition is false. 
In summary, control flow statements and decision-making structures allow programmers to create flexible and responsive programs that can adapt their behavior based on specific conditions during execution. 
### If Statement, IF ELSE statement, Nested If Statement 
* An if statement consists of a Boolean expression followed by one or more statements.  
* If the Boolean expression evaluates to true then the block of code inside the if statement (Statements) will be executed.  
* If the Boolean expression evaluates to false, then the block of code inside the if statement (Statements) will not be executed 

### IF ELSE Statement:
An if statement can be followed by an optional else statement, which executes when the Boolean expression is false. The diagram below shows the flow of an if else statement. 
As you can see the are two code blocks to be executed, the block for if the condition is true and a block for when the condition false. 
### Nested If Statement:
An if statement can be followed by an optional else if...else statement, which is very useful to test various conditions using single if...else if statement. You have as many else if as the number of you possible conditions 
* When using if, else if, else statements there are a few points to keep in mind. 
* An if can have zero or one else's and it must come after any else if's. 
* An if can have zero to many else if's and they must come before the else. 
* Once an else if succeeds, none of the remaining else if's or else's will be tested. 
### Switch statement and the Tenary (?) operator:
#### SWITCH STATEMENT:
A switch statement allows a variable to be tested for equality against a list of values. Each value is called a case, and the variable being switched on is checked for each case. 
Switch case statement is used when we have number of options (or choices) and we may need to perform a different task for each choice. 
##### General rules to a switch statement are: 
* The variable used in a switch statement can only be integers, convertible integers (byte, short, char), strings and enums. 
* You can have any number of case statements within a switch. Each case is followed by the value to be compared to and a colon. 
* The value for a case must be the same data type as the variable in the switch and it must be a constant or a literal. 
* When the variable being switched on is equal to a case, the statements following that case will execute until a break statement is reached. 
* When a break statement is reached, the switch terminates, and the flow of control jumps to the next line following the switch statement. 
* Not every case needs to contain a break. If no break appears, the flow of control will fall through to subsequent cases until a break is reached. 
* A switch statement can have an optional default case, which must appear at the end of the switch. The default case can be used for performing a task when none of the cases is true. No break is needed in the default case. 
#### The tenary (?) operator:
The tenary operator only caters for two outcomes. Like the IF ELSE statement evaluates for the true or false only. It can only be used in place of if else statement. 
Syntax:
(expression1)? expression2: expression3; 
Where expression1, expression2, and expression3 are expressions. Notice the use and placement of the colon. 
To determine the value of the whole expression, initially exp1 is evaluated. 
If the value of exp1 is true, then the value of Exp2 will be the value of the whole expression. 
If the value of exp1 is false, then Exp3 is evaluated and its value becomes the value of the entire expression. 

## Day 5: 
## Java Modifiers: 

### JAVA MODIFIERS:

#### Java Identifiers:

* In Java, identifiers are names given to various program elements such as classes, variables, methods, and labels.  
* Identifiers serve as the means to uniquely identify and distinguish these elements within a Java program. 
* Identifiers are the names of variables, methods, classes, packages and interfaces. Unlike literals they are not the things themselves, just ways of referring to them.  
* In the HelloWorld program, HelloWorld,  args, main and println are identifiers.

#### Composition of Identifiers: 
Characters Allowed: Identifiers in Java can be composed of letters (a-z, A-Z), numbers (0-9), the underscore (_), and the dollar sign ($). 
Starting Character: Identifiers must begin with a letter, underscore, or dollar sign. 

#### CamelCase Convention: 
Definition: CamelCase is a naming convention where compound words or phrases are written such that each word or abbreviation begins with a capital letter (except the first word, which starts with a lowercase letter). 
Example: myVariableName, calculateTotalAmount, employeeDetails 


 #### Java Modifiers: 
Definition: Modifiers in Java are keywords that modify the meanings of identifiers such as classes, methods, variables, etc. 

#### Types of Modifiers: 

##### *Java Access Modifiers: 
Control the visibility of classes, methods, and variables. Examples include public, private, protected. 

##### * Non-Access Modifiers:
Provide additional information about classes, methods, and variables. Examples include static, final, abstract. 

###### Usage of Modifiers: 
Application: Modifiers are used by including their keyword in the definition of a class, method, or variable. They precede the rest of the statement. 

In summary, identifiers in Java follow specific rules regarding their composition, and CamelCase is a common naming convention. Modifiers, both access and non-access, are keywords that can be applied to identifiers to modify their behavior or visibility in a Java program. Using these conventions and modifiers helps in writing clear, readable, and maintainable code. 

                                                                      --- END OF WEEK 1 ---

## Week 2: 
## Day 1:
## Git: 
### What is GIT?
* 	Git is a modern and widely used distributed version control system in the world.
* 	Developed to manage projects with high speed and efficiency. T
* 	The version control system allows us to monitor and work together with our team members at the same workspace.
*	Git is an open-source distributed version control system
* It is developed to co-ordinate the work among the developers. 
*	The version control allows us to track and work together with our team members at the same workspace.
*	Git is foundation of many services like GitHub and GitLab, but we can use Git without using any other Git services. Git can be used privately and publicly.

### GIT VERSION CONTROL:
*	A version control system is a software that tracks changes to a file or set of files over time so that you can recall specific versions later.
*	It also allows you to work together with other programmers or developers. 
*	The version control system is a collection of software tools that help a team to manage changes in a source code.
*	It uses a special kind of database to keep track of every modification to the code.
*	There are several git hosting services (remote repository) in the market. Some are free and some are commercial. These include GitHub, Bitbucket and Gitlab

### BENEFITS OF GIT:
*	A version control application allows us to keep track of all the changes that we make in the files of our project(s). 
*	Every time we make changes in files of an existing project, we can push those changes to a repository.
*	Other developers are allowed to pull your changes from the repository and continue to work with the updates that you added to the project files.
Main benefits of GIT include the following
*	Saves time-every commands takes seconds to execute compared to login in on Github and navigating  its features
*	Supports offline working-one can work locally if they have connectivity issues
*	Undo mistakes
*	Track changes=make use of Log, Status to keep track of any changes that have been applied

## Day 2:
## Git Tools and Packages: 
### Git Tools:
•	Git comes with some tools like Git Bash, Git GUI to provide the interface between machine and user. It supports inbuilt as well as third-party tools.
•	Git comes with built-in GUI tools like git bash, git-gui, and gitk for committing and browsing. It also supports several third-party tools for users looking for platform-specific experience.

### Git Package Tools: 
•	Git provides powerful functionality tools such as commands, command line, Git GUI
•	Git Bash is a command-line interface (CLI) application designed for the Windows operating system. It serves as a command-line interface for Git, a distributed version control system widely used for source code management and collaboration in software development.

### Git Bash:
•	Git Command Line for Windows: Git Bash is specifically tailored for the Windows environment. It allows users to interact with Git repositories using a command-line interface, similar to the way Git is used on Linux and macOS systems.
•	Emulation Layer: Git Bash provides an emulation layer that simulates the experience of using Git on a Unix-like system within the Windows environment. This is achieved by incorporating the Bash (Bourne Again Shell) shell, which is a common shell on Unix-like operating systems.
•	Bash as the Default Shell: Bash, in the context of Git Bash, stands for Bourne Again Shell. It is a standard default shell on Linux and macOS. In a broader sense, a shell is a terminal application that allows users to interact with the operating system through command-line instructions.
•	Git Package Installer: When you install Git on a Windows operating system using the Git package installer, it includes not only the Git version control system but also the Git Bash tool. This tool combines the Git command-line capabilities with the Bash shell and utilities.
•	Accessing Git Bash: After installing Git on Windows, you can access Git Bash by right-clicking on a folder in Windows Explorer. This opens a context menu that includes an option to open Git Bash within the selected folder. Once opened, Git Bash provides a command-line interface where you can execute Git commands and Bash commands.
•	In summary, Git Bash is a convenient tool for Windows users who want to use Git via the command line. It brings the Git experience to the Windows environment by incorporating the Bash shell and utilities, allowing users to work with Git repositories in a familiar and powerful command-line interface.

### Git Bash Command: 
•	Git Bash Commands refer to the additional shell commands that come bundled with Git Bash, a command-line interface for Git on Windows. These commands are stored in the /usr/bin directory within the Git Bash emulation. Git Bash aims to provide a robust shell experience on Windows by incorporating a set of essential shell commands commonly found on Unix-like systems.

### Shell Commands: 
•	Location: The additional commands are stored in the /usr/bin directory. This directory contains executable files for various shell commands that enhance the functionality of Git Bash.
•	Examples of Commands:
•	ssh: Used for securely connecting to remote servers or systems.
•	scp: Stands for "secure copy." It is used for secure file copying between a local host and a remote host.
•	cat: Used to concatenate and display the content of files.
•	find: A command-line utility for searching files and directories.

### Essential Git Commands: 
•	Git Bash includes the full set of Git core commands, allowing users to interact with Git repositories seamlessly. These commands are fundamental to version control using Git. Some examples include:
•	git clone: Used to clone a repository into a new directory.
•	git commit: Commits changes to the repository with a descriptive message.
•	git checkout: Switches between branches or restores working tree files.
•	git push: Pushes local changes to a remote repository.
•	Using Git Bash Commands, users can harness the power of both the Git command line and additional shell commands on a Windows system. This provides a flexible and comprehensive environment for working with Git repositories and performing various shell-related tasks. The inclusion of a GUI option further enhances the user experience, catering to users who prefer a visual interface for their version control workflows.

### Git GUI:
•	Git GUI, or Git Graphical User Interface, is a visual tool that provides an alternative to using the Git command line (Git Bash) for interacting with Git repositories. It offers a graphical representation of Git commands and includes visual diff tools for comparing changes. Git GUI is particularly helpful for users who prefer a visual interface or find it more convenient than using the command line for certain tasks.
•	In addition to the command-line interface provided by Git Bash, Git also comes with a graphical user interface (GUI). The Git GUI is a visual tool that allows users to perform Git operations using a graphical interface rather than the command line.
•	The Git GUI provides a more user-friendly way to manage repositories, visualize changes, and perform version control tasks.
•	Graphical Representation: Git GUI offers a visual representation of Git commands and operations. 
•	This includes a graphical history of commits, branches, and other aspects of the repository. This visual representation can make it easier for users to understand the structure and history of a Git project.
•	Visual Diff Tools: Git GUI includes visual diff tools that allow users to compare changes between different versions of files. This can be useful for reviewing changes before committing them, resolving conflicts, or understanding the differences between branches.

### Accessing the GUI:
•	Right-Click in Windows Explorer: One of the convenient ways to access Git GUI is by right-clicking on a folder or location in Windows Explorer. This opens a context menu that includes an option to open Git GUI for the selected location. This allows users to navigate to a specific repository and launch the graphical interface with ease.
•	Command Line: Users can also access Git GUI through the command line by typing the following command: git gui
•	Executing this command launches the Git GUI application, providing a visual interface for Git operations.
•	User-Friendly Interface: Git GUI is designed to be user-friendly, especially for those who may not be comfortable with the command-line interface. It allows users to perform common Git operations with a point-and-click approach, reducing the need for manual command entry.
•	Parallel to Command Line: While Git GUI provides a graphical interface, it doesn't replace the Git command line; rather, it works in parallel with it. Users can choose the interface that suits their preferences and the specific requirements of their tasks.
•	In summary, Git GUI is a valuable tool for users who prefer a visual representation of Git operations and a point-and-click interface. It complements Git Bash by offering an alternative way to interact with Git repositories, making version control more accessible to a wider range of users.

### GitK:
•	gitk is a graphical history viewer tool for Git, providing a visual representation of a project's history and allowing users to explore changes and commits. It serves as a robust graphical user interface (GUI) that builds on top of Git's log and grep commands, making it easier for users to navigate and understand the history of a Git repository.
•	Graphical History Viewer:
•	gitk is designed to be a graphical tool that allows users to visually explore the history of a Git repository. It provides a graphical representation of commits, branches, and other Git-related information.
•	Built on Git Commands:
•	Internally, gitk relies on Git commands such as git log and git grep to gather information about the repository's history. It consolidates and presents this information in a graphical format.

### Command-Line Innovation: 
•	Users can invoke gitk from the command line by navigating to the root directory of a Git repository and typing the following command: $ gitk [git log options]
•	The optional [git log options] allow users to customize the information displayed in the history view.

### Finding Past-Events: 
•	gitk is particularly useful for finding specific events or changes that occurred in the past. Users can navigate through the graphical interface to inspect commits, view commit messages, and understand the evolution of the project over time.

### Visualizing Project History: 
•	The tool is instrumental in visualizing the project's history, making it easier to understand the relationships between different commits, branches, and merges. This visual representation can be more intuitive than examining the same information in a text-based format.

### Interactive Interface: 
•	gitk provides an interactive interface where users can click on individual commits to view details, explore branches, and navigate through the project's timeline. This makes it easier to comprehend complex branching and merging scenarios.
•	In summary, gitk is a powerful graphical history viewer tool that enhances the Git experience by providing a visual interface for exploring the history of a Git repository. Whether you need to review past changes, understand branching patterns, or investigate commit details, gitk offers a convenient and user-friendly way to interact with the historical data in your Git projects.

## Git Terminologies: 

### Branch: 
•	Definition: A branch is a version of the repository that diverges from the main working project. It allows for parallel development and experimentation.
•	Operations: Branches can be renamed, listed, deleted, and more.


### Checkout: 
•	Definition: The act of switching between different versions of a target entity, typically used for switching between branches.
•	Command: git checkout is used to switch between branches in a repository.

### Cherry-Picking:
•	Definition: Applying a specific commit from one branch to another, useful for selectively incorporating changes. In case you made a mistake and committed a change into the wrong branch, but do not want to merge the whole branch
•	Use Case: Useful for reverting a commit from one branch and applying it to another.

### Clone:
•	Definition: Creating a local copy of a target repository.
•	Command: git clone is used to clone a repository, creating a local copy from a specified URL.

### Fetch: 
•	Definition: Fetches branches and tags from other repositories, updating remote-tracking branches.
•	Purpose: Keeps the local repository up-to-date with changes from remote repositories.

### HEAD: 
•	Definition: Staging area between the working directory and repository, used to build up changes for committing.
•	Purpose: Allows selective staging of changes before committing.


### Index: 
•	Definition: Staging area between the working directory and repository, used to build up changes for committing.
•	Purpose: Allows selective staging of changes before committing.

### Master:
•	Definition: Default branch in Git, commonly named "master."
•	Usage: Initial branch after cloning a repository.

### Merge: 
•	Definition: Process of combining diverged histories to integrate changes into a single branch.
•	Command: git merge integrates changes from one branch into another.

### Origin: 
•	Definition: Reference to the remote repository from which the project was initially cloned.
•	Usage: Used instead of the original repository URL for referencing.

### 	Pull/Pull Request:
•	Pull: Receiving data from a remote repository.
•	Pull Request: Notification to team members that a feature branch is ready for review and merging.

### 	Push:
•	Definition: Uploading local repository content to a remote repository.
•	Caution: Careful consideration needed as pushing can overwrite changes.

### Rebase:
•	Definition: Process of moving or combining commits to a new base commit.
•	Use Case: Helps visualize and streamline the feature branching workflow.

### Remote:
•	Definition: Concerned with the remote repository, a shared repository for team collaboration.
•	Content: Typically contains Git versioning data rather than a file tree.

### Repository:
•	Definition: Data structure used by version control systems to store metadata and project-related data.
•	Representation: Considered as the project folder in Git.

 ### Stashing:
•	Definition: Temporarily saving changes to switch branches without committing incomplete work.
•	Command: git stash is used to stash changes.

### Tag:
•	Definition: Marks a specific point in Git history, used for important commit stages.
•	Types: Light-weighted tag and Annotated tag.

### Upstream and Downstream:
•	Definition: Reference to the direction of repository integration.
•	Upstream: Cloned repository (origin). Downstream: Projects integrating your work.

### Git Revert:
•	Definition: Reverts a specific commit using git revert.
•	Type: An undo command, but not a traditional undo alternative.

### Git Reset:
•	Definition: Undoing changes in Git, with forms like Soft, Mixed, and Hard reset.
•	Command: git reset is used for resetting changes.

### Git Ignore:
•	Definition: Specifies intentionally untracked files that Git should ignore.
•	Effect: Does not affect files already tracked by Git.

### Git Diff:
•	Definition: Multi-use Git command to show changes between commits, branches, commits, and working tree.
•	Usage: Provides a detailed view of differences in Git data sources.

### Git Cheat Sheet:
•	Definition: A summary of Git commands for quick reference.
•	Purpose: A quick guide for users to recall essential Git commands.


### Git Flow:
•	Definition: A branching model for Git, aiding collaboration and scaling development teams.
•	Components: A collection of Git commands for repository operations.

### Git Squash:
•	Definition: Squashing multiple commits into one for cleaner commit history.
•	Use Case: Grouping specific changes before merging.

### Git Rm:
•	Definition: Removes individual files or a collection of files from the Git index.
•	Effect: Tracked files are removed from both the working directory and staging index.

### 	Git Fork:
•	Definition: Creating a rough copy of a repository for testing and debugging without affecting the original project.
•	Usage: Useful for proposing changes and resolving issues in a separate copy.
•	Understanding these Git terms is crucial for mastering version control and collaborating effectively on software development projects.

## Day 3: 
## Git Basic Commands:
Git commands are all run only on Git command line. These commands execute specific tasks on git.

### git config:
Purpose: Used to set configuration options for Git at both system and local levels.
Example: git config --global user.name "Your Name"
### 	git init:
Purpose: Initializes a new Git repository, creating the necessary data structures and files.
Example: git init
### git clone:
	Purpose: Creates a copy of a remote repository on your local machine.
	Example: git clone <repository URL>
### 	git add:
	Purpose: Adds changes in the working directory to the staging area in preparation for a commit.
	Example: git add file.txt
### 	git commit:
	Purpose: Records changes in the repository along with a commit message.
	Example: git commit -m "Your commit message"
### git status:
	Purpose: Displays the status of changes as untracked, modified, or staged.
	Example: git status
### 	git push:
	Purpose: Uploads local repository content to a remote repository.
	Example: git push origin master
### git pull:
	Purpose: Fetches changes from a remote repository and merges them into the local repository.
	Example: git pull origin master
### git branch:
	Purpose: Lists, creates, or deletes branches in the repository.
	Example: git branch (to list branches) or git branch new-feature (to create a new branch named "new-feature")

### 	git merge:
	Purpose: Combines changes from different branches into the current branch.
	Example: git merge feature-branch
### 	git log:
	Purpose: Displays a log of commits in reverse chronological order.
	Example: git log
### git remote:
	Purpose: Manages connections to remote repositories.
	Example: git remote -v (to view remote repositories and their URLs)
	These commands form the core set of actions in Git, enabling version control, collaboration, and tracking changes in a software project. Each command plays a specific role in different stages of the Git workflow, from initialization (git init) to fetching and integrating changes (git pull and git merge). Understanding these commands is essential for efficient and effective use of Git in software development.

## Staging and Commit:
### Git Add:
	Purpose: Adds file contents to the Index (Staging Area) for the next commit.
	Usage: $ git add <file_name> adds a specific file; $ git add -A or $ git add . adds all files.
	Additional Options:
	--ignore-removal: Stages only updated and newly created files.
	-u: Stages only modified and deleted files.
	Files can also be added by specifying a pattern, e.g., $ git add *.java.
### Git Commit:
	Purpose: Records changes in the repository with a commit message.
	Usage:
	$ git commit opens a text editor for a commit message.
	$ git commit -a commits all changes previously added, excluding newly created files.
	$ git commit -m "Commit message." provides a commit message inline.
	$ git commit --amend allows editing the last commit's message.
### 	Git Clone:
	Purpose: Creates a local copy of a remote repository.
	Usage: $ git clone <repository_URL>
	Additional Option:
	-b <branch_name>: Clones a specific branch.
### 	Git Fork:
	Definition: A fork is a copy of a repository, often used for experimentation without affecting the original project.
	Usage: Done through Git service platforms like GitHub.
	Steps to Fork on GitHub:
	Log in to GitHub.
	Find the repository to fork.
	Click "Fork" in the upper right.
	Notes: Forking is commonly used for contributing to open-source projects, allowing users to experiment, make changes, and propose those changes back to the original project through pull requests.
	These Git commands are fundamental for version control, collaboration, and contributing to projects. git add stages changes, git commit records them, git clone creates local copies, and forking is a method for safe experimentation and contribution on Git service platforms like GitHub.

## Day 4: 
## Git log and Git Checkout:
Here you can inspect, and undo changes. 
### Git Log: 
	Purpose: Git log is a command-line utility that allows users to review and read the history of a Git repository. It displays a detailed log of commits, including commit hashes, author metadata, commit date, and commit messages.
	Usage: $ git log provides a comprehensive list of recent commits with their unique identifiers, authors, dates, and commit messages.
## 	Git Log Stat:
	Purpose: The --stat option in git log is used to display additional information about modified files, including the number of lines added or removed and a summary line of total changes.
	Usage: $ git log --stat provides a more detailed view of the modifications made in each commit.

## Git Log P or Patch:
	Purpose: The --patch option in git log, or simply using $ git log -p, displays the files that have been modified, along with the location of added, removed, and updated lines, providing a detailed view of specific changes made.
	Usage: $ git log --patch or $ git log -p shows a patch-style output for a more in-depth understanding of modifications.

## Git Checkout: 
	Purpose: Git checkout is used to switch between different versions of a target entity, such as files, commits, or branches, in a Git repository. It updates the working directory to match the selected version.
	Operations:
	Switch Branch: $ git checkout <branchname> switches to the specified branch.
	Create and Switch Branch: $ git checkout -b <branchname> creates a new branch and switches to it simultaneously.
	Checkout Remote Branch:
	Fetch contents: $ git fetch
	Checkout: $ git checkout <remotebranch>
	Extra Notes:
	Be cautious with the git checkout command, as it operates on files, commits, and branches, and there is no undo option.
	Operations like creating and switching branches (-b option) or checking out remote branches involve combining git branch and git checkout commands.
	Git log is crucial for navigating and understanding the history of a Git repository, and options like --stat and --patch enhance the information displayed.

### COLLABORATING: 
Here you can pull, fetch, and push. 

### 	Git Fetch:
	Purpose: Downloads commits, objects, and refs from another repository. Fetches branches and tags from one or more repositories.
	Usage: $ git fetch <repository_URL> fetches updates from a specific repository URL.
	$ git fetch <branch_URL> <branch_name> fetches a specific branch from a repository.
	$ git fetch --all fetches all branches simultaneously from a remote repository.
	Notes: Remote-tracking branches are updated to keep track of the remote repository's history.
### 	Git Pull / Pull Request:
#### 	Git Pull:
	Purpose: Receives data from GitHub, fetching and merging changes from the remote server to the working directory.
	Usage: $ git pull <options> [<repository_URL><refspec>...]
	<options>: Additional commands like -q (quiet), -v (verbose), -e (edit), etc.
	<repository_URL>: URL of the remote repository.
	Notes: Combines fetch and merge, updating local branches with remote-tracking branches.
### Pull Request:
	Purpose: Notifies team members of completed features. A developer files a pull request to review and merge the feature branch into the master branch.
	Process: Developer initiates a pull request via their remote server account, signaling team members to review and merge the code.
### Git Push:
	Purpose: Uploads local repository content to a remote repository, transferring commits.
	Usage: $ git push <options> [<Remote_URL><branch_name><refspec>...]
	<options>: Various options such as --all, --prune, --mirror, --dry-run, --tags, --delete, -u, etc.
	<Remote_URL>: URL or name of the remote repository.
	Options Overview:
	--all: Pushes all branches.
	--prune: Removes remote branches without local counterparts.
	--mirror: Mirrors the repository to the remote, updating or creating local refs.
	--dry-run: Tests commands without updating the repository.
	--tags: Pushes all local tags.
	--delete: Deletes the specified branch.
	-u: Creates an upstream tracking connection for the first push.
### Git Force Push:
	Purpose: Forces push local repository to remote without dealing with conflicts.
	Usage: $ git push <remote><branch> -f or $ git push <remote><branch> --force
### Safe Force Push:
	Uses --force-with-lease to fail if there are unexpected new commits on the remote.
	Usage: $ git push <remote><branch> --force-with-lease
	Delete a Remote Branch:
	Purpose: Deletes a remote branch from the command line.
	Usage: $ git push origin --delete <branch_name> removes a specific remote branch.
	These Git collaboration commands facilitate sharing code among developers, including fetching updates, pulling changes, and pushing local commits to remote repositories. Pull requests provide a structured process for code review and integration. Force push and safe force push options are available for updating remote branches, and deleting remote branches can be accomplished using the push command.




                                                 --- END OF WEEK 2 ---
 

 
