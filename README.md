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

 

 
