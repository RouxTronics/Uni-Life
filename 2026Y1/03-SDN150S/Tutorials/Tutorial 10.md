---
title: Tutorial 10
course: SDN150S
tags:
  - java
  - cput/sdn150s
---
# Questions 
## Q.1

> What does the command ‘javac filename.java’ do?

The command javac filename.java compiles the Java source code (.java file) into Java bytecode (.class file), which can then be executed by the Java Virtual Machine (JVM).

**Answer**: `Compiles the Java source file into bytecode.`

## Q.2 

> Which Java framework is commonly used for GUI development?

**JavaFX** is the modern framework recommended for developing rich graphical user interfaces (GUIs) in Java, featuring built-in support for modern CSS styling, FXML layout separation, and 3D graphics.

**Answer**: `JavaFX`

## Q.3

>What does the method nextLine() do in the Scanner class?

The nextLine() method of the Scanner class reads user input as a string from the current position up to the end of the line (until the Enter key / newline character \n is encountered).

**Answer**: `Reads a full line of input from the user until Enter is pressed.`


## Q.4 

> Which of the following is the correct way to declare a method in Java?

In Java, method declarations follow the structure: access modifier (`public`), return type (`void`), method name (`myMethod`), followed by parameters in parentheses and the body in braces:

```java 
public void myMethod(){
	 // method body
}
```

**Answer**: `public void myMethod() {}`

## Q.5 

> What is encapsulation in object-oriented programming?

**Encapsulation** is the core OOP principle of bundling data (fields/attributes) and the methods that operate on that data into a single unit (a class), while restricting direct access to some of the object's components (typically using private access modifiers and getter/setter methods).


**Answer**: `Bundling data and methods that operate on that data into a single unit.`


## Q.6 

> What is the role of the JVM in Java?

The primary role of the JVM (Java Virtual Machine) is to **execute Java bytecode**.

| Prompts                                      | Answers       |
| -------------------------------------------- | ------------- |
| Executes Java bytecode.                      | JVM           |
| Translates Java code to machine code.        | Compiler      |
| Handles syntax errors during compile time.   | Compiler      |
| Provides a user interface for Java programs. | GUI framework |
## Q.7 

> Which of the following statements is true about Java?

When Java source code is compiled, it is converted into platform-neutral bytecode (.class files). This bytecode can then be executed on any operating system that has a compatible Java Virtual Machine (JVM) installed, following the "Write Once, Run Anywhere" principle.

**Answer**: `Java is platform-independent due to its bytecode.`

## Q.8 

| Prompts<br>                                | Answers        |
| ------------------------------------------ | -------------- |
| Bundling data and methods together.        | Encapsulation  |
| Inheriting properties from a parent class. | Inheritance    |
| Using multiple methods for a single task.  | Polymorphism   |
| Preventing data access from outside.       | Access control |

## Q.9 


| Prompts<br>                           | Answers   |
| ------------------------------------- | --------- |
| Blueprint for creating objects        | Class     |
| A specific instance of an object.     | Object    |
| A method to execute tasks.            | Method    |
| A collection of primitive data types. | Primitive |
## Q.10

> Which of the following is NOT a keyword in Java?

- **`static`**: A keyword used to declare members (variables/methods) that belong to the class rather than instances.
    
- **`public`**: An access modifier keyword that makes a class, method, or variable accessible from any other class.
    
- **`void`**: A keyword used to specify that a method does not return any value.

**Answer**: `classical`

## Q.11

> What is the main method in a Java program?

The `main` method (`public static void main(String[] args)`) serves as the **entry point for program execution** in Java; it is where the Java Virtual Machine (JVM) starts running the application.

**Answer**: `The entry point for program execution.`

## Q.12 

>Which of the following cannot be used as an identifier in Java?

In Java, identifier naming rules state that:

- Identifiers **cannot start with a digit** (0–9).
    
- Identifiers can begin with a letter (A–Z or a–z), a currency symbol (e.g., `$`), or an underscore (`_`).
    
- Subsequent characters can include digits, letters, `$`, or `_`.

**Answer**: `3variable`

## Q.13 

> What will be the output of the following code snippet? 
> `System.out.println(5 + 10);`

**Answer**: `15`
## Q.14 

> What is the correct way to create an instance of a Scanner?

 `Scanner sc = new Scanner(System.in);` $\rightarrow$ **True** _(This uses the `new` keyword with the standard `System.in` constructor)_

- Rest is False

## Q.15 

> Which class is commonly used for input operations in Java? 

**(Scanner):** Commonly used for reading formatted input (strings, integers, doubles) from standard input (`System.in`).

**Answer**: `Scanner`

## Q.16

> What will the following code output? System.out.print("Hello"); System.out.print("World");

`System.out.print()` outputs text to the console without adding a newline or automatic spacing. Since neither call includes spaces or newlines, the output is printed directly next to each other as **`HelloWorld`**.


**Answer**: `HelloWorld`

## Q.17 
> In the context of Java, what does JVM stand for?

**Answer**: `Java Virtual Machine`

## Q.18 

> What is the purpose of the` System.out.println() `method?

**Answer**: `To print a message to the console followed by a new line.`

