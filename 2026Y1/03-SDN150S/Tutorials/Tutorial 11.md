---
title: Tutorial 11 - SDN150S
type: Tutorial
categories: SDN150S
tags:
---
# Overview 

First Attempt: `16.5 / 20`
Second Attempt: `17 / 20`
# Questions 
## Q.1 - What is the role of methods in a Java class?

| Prompts                                                         | Answers                          |
| --------------------------------------------------------------- | -------------------------------- |
| Methods define the behaviour of objects created from the class. | Yes, that's correct.             |
| Methods are used strictly for data storage                      | No, that's incorrect.            |
| Methods can only return void values.                            | No, methods can return any type. |
| Methods can be defined only once in a class.                    | No, methods can be overloaded.   |
## Q.2 - What happens when you try to instantiate an abstract class?

| Prompts                                                 | Answers                                        |
| ------------------------------------------------------- | ---------------------------------------------- |
| It results in a compilation error.                      | Yes, you cannot instantiate an abstract class. |
| You will create an object of the class successfully.    | No, that's not a result.                       |
| You are prompted to create a static method instead.     | No, that's unrelated to instantiation.         |
| The class will automatically implement default methods. | No, that's not a result.                       |
## Q.3 - What is the access level of a class that has no access modifier declared?

| Prompts                                                              | Answers                                                         |
| -------------------------------------------------------------------- | --------------------------------------------------------------- |
| Package-private; accessible only within its own package.             | Yes, that's package-private access.                             |
| Public; accessible from everywhere.                                  | No, that's incorrect.                                           |
| Private; only accessible within its own class.                       | No, it cannot be private if no modifier is declared.            |
| Protected; accessible to subclasses and classes in the same package. | No, that only applies to explicitly declared protected classes. |
## Q.4 -  What is the significance of the 'public' access modifier in a class declaration?

Here is how each option breaks down:

- **Option A (Correct):** The `public` access modifier removes package-level restriction, allowing any class in any package to access and instantiate the class.
    
- **Option B:** Making a class abstract requires the `abstract` keyword, not `public`.
    
- **Option C:** Restricting instantiation is typically done by making constructors `private` or using the `abstract` keyword.
    
- **Option D:** Package-only access is achieved by omitting the access modifier altogether (often referred to as _default_ or _package-private_ access).


**Answer**:  `It allows the class to be accessible from other classes.`

## Q.5 - What is an instance variable?

Here is how each option breaks down:

- **Option B (Correct):** An instance variable is declared inside a class but outside any method. Every time an object (instance) of that class is created, it gets its own separate copy of that variable, holding its own state.
    
- **Option A:** Pure object-oriented languages like Java or C# do not allow variables to be defined outside of a class.
    
- **Option C:** Variables accessed statically are marked with the `static` keyword and belong to the class itself, not to specific instances.
    
- **Option D:** A variable shared across all instances of a class is a **static variable** (or class variable), which exists as a single copy in memory regardless of how many objects are instantiated.

**Answer**: `A variable defined in a class for each object instance.`

## Q.6 - What happens if a class contains multiple constructors in Java?

What is the relationship between classes and objects in Java?
Here is a breakdown of why this happens:

- **Option C (Correct):** Having multiple constructors with the same name (the class name) but different parameter lists within the same class is known as **constructor overloading**. Java determines which constructor to call based on the number and types of arguments passed when creating an object.
    
- **Option A:** This is completely valid Java syntax, so the program compiles without issue.
    
- **Option B:** Java recognizes all validly declared constructors, not just the first one.
    
- **Option D:** The constructors you explicitly define will exist and be available for use. (However, providing explicit constructors does mean Java will no longer generate the default, no-argument constructor automatically.)

**Answer**: `Constructor overloading occurs.`

## Q.7 - What is the relationship between classes and objects in Java?


- **Option B (Correct):** A **class** serves as the blueprint, template, or design, while an **object** is a concrete instance created from that blueprint residing in memory.
    
- **Option A:** This is reversed—objects are instances of classes, not the other way around.
    
- **Option C & D:** While both statement C and statement D express true core Java concepts in isolation (a class definition exists in code without needing active objects, and objects require a class definition to be created), in standard multiple-choice assessments testing the fundamental OOP definition, **Option B** directly defines the primary relationship between the two terms.

**Answer**: `An object is an instance of a class.`

## Q.8 - Which of the following statements correctly declares an instance variable in Java?

**Answer**: `String name;`

## Q.9 -  How do you create an object of a class named 'Dog'?

Here is a breakdown of why this option is correct and why the others are invalid in Java:

- **Option C (Correct):** Creating an object requires three parts: declaring the variable type and name (`Dog myDog`), using the `new` keyword to allocate memory, and invoking the class constructor with parentheses (`Dog()`).
    
- **Option A:** This looks like a function declaration (or C++ object instantiation), which is invalid for instantiating an object in Java.
    
- **Option B:** Missing the parentheses `()` after the class name, which are required to invoke the constructor.
    
- **Option D:** Places the `new` keyword before the class type declaration, which is invalid Java syntax.

**Answer**: `Dog myDog = new Dog();`

## Q.10 

>Which access modifier restricts a class from being instantiated from outside its own definition?

- **Option B (Correct):** Making a class's constructor `private` prevents any code outside the class definition from using `new` to instantiate it. This design pattern is commonly used for Singleton patterns or utility classes (like `java.lang.Math`).
    
- **Option A (default):** Allows instantiation by any class within the same package.
    
- **Option C (public):** Allows instantiation from any class across any package.
    
- **Option D (protected):** Allows instantiation by classes within the same package and by subclasses in other packages.

**Answer**: `private`

## Q.11 

> What does encapsulation mean in Java?


| Prompts                                                                                       | Answers                                   |
| --------------------------------------------------------------------------------------------- | ----------------------------------------- |
| Hiding the internal state and requiring all interaction to occur through an object's methods. | Yes, that's the essence of encapsulation. |
| Keeping all class data public for accessibility.                                              | No, encapsulation focuses on hiding data. |
| Sharing data across all classes in a package.                                                 | No, that weakens encapsulation.           |
| Allowing free access to all methods in a class.                                               | No, that opposes encapsulation.           |

## Q.12 

> In the context of Java, what does the Singleton design pattern ensure?

Here is a quick breakdown of the design pattern:

- **Option A (Correct):** The Singleton pattern restricts class instantiation so that only one single instance of the class exists in the Java Virtual Machine (JVM), providing a global point of access to it.
    
- **Option B:** Creating multiple instances is standard object-oriented behavior and the exact opposite of what the Singleton pattern enforces.
    
- **Option C:** While Java requires constructors to instantiate objects, this is a language rule, not the core goal of the Singleton pattern.
    
- **Option D:** Singleton implementations actually rely heavily on a public `static` method (e.g., `getInstance()`) to grant access to the single instance.

**Answer**: `Only one instance of a class is created.`


## Q.13 - What happens if a class does not define any constructor?

| Prompts                                                       | Answers                                        |
| ------------------------------------------------------------- | ---------------------------------------------- |
| A default constructor is automatically provided by Java.      | Yes, that's correct.                           |
| The class will not compile.                                   | No, not necessarily                            |
| The programmer must define at least one constructor manually. | No, there is no requirement for a constructor. |
| The class becomes abstract by default.                        | No, that is unrelated to constructors.         |
## Q.14 

> What method is called automatically when an object is created?

Here is a quick breakdown of why this happens:

- **Option C (Correct):** A constructor is a special block of code that is invoked automatically when an object is instantiated using the `new` keyword. Its primary role is to initialize the object's instance variables and set up its state.
    
- **Option A:** An instance variable holds state/data for an object; it is not a executable method that runs automatically.
    
- **Option B:** A regular method must be invoked explicitly (e.g., `object.methodName()`) after the object is created.
    
- **Option D:** A static block executes automatically when the class is loaded into memory by the JVM, not when individual objects are created.

**Answer**: `A constructor`

## Q.15 

> What is the function of the 'this' keyword in Java constructors?


Here is how each option breaks down:

- **Option B (Correct):** Within a constructor or instance method, the `this` keyword acts as a reference variable pointing directly to the current object instance being created or manipulated. In constructors, it is commonly used to distinguish instance variables from parameter names with identical identifiers (e.g., `this.name = name;`) or to chain constructors (e.g., `this();`).
    
- **Option A:** Referring to the parent (superclass) instance is done using the `super` keyword, not `this`.
    
- **Option C:** While constructor chaining using `this()` works with overloaded constructors, the keyword itself does not perform or define method overloading.
    
- **Option D:** New objects are created using the `new` keyword, which allocates memory and invokes the constructor.

**Answer**: `It refers to the current object instance.`


## Q.16 

> What is the output of trying to access a private variable from outside its class?


| Prompts                                       | Answers                                                |
| --------------------------------------------- | ------------------------------------------------------ |
| It results in a compilation error             | Yes, private variables cannot be accessed from outside |
| It shows the variable's value in the console. | No, that's not correct.                                |
| It would return a default value.              | No, that is inaccurate.                                |
| It prompts the user for a value.              | No, this is incorrect behaviour.                       |
## Q.17 

> In which of the following scenarios would you use a private constructor?

Here is why:

- **Option D (Correct):** A `private` constructor prevents other classes from directly instantiating the class using `new`. This is a core requirement of the **Singleton pattern**, ensuring the class controls its own instantiation and provides only a single global instance.
    
- **Option A:** Making a constructor `private` actually **prevents** subclassing because child classes must call a parent constructor (via `super()`), which they cannot access if it is private.
    
- **Option B:** Instance variables are declared directly inside the class body, not within constructors.
    
- **Option C:** Interfaces do not have constructors at all because they cannot be instantiated directly.

**Answer**: `To implement the Singleton pattern.`


## Q.18 - What must a public class name match in terms of its source file?

Here is why:

- **Option C (Correct):** In Java, if a class is declared as `public`, the source code file **must** be named identically to the class, including exact case sensitivity, with a `.java` extension (e.g., `public class Person` must be stored in `Person.java`).
    
- **Option A:** Classes can certainly be declared as `public`.
    
- **Option B:** File naming is strictly enforced for public classes; it cannot be named arbitrarily.
    
- **Option D:** While a single `.java` file can contain multiple classes, only _one_ of those classes can be declared `public`, and the file name must match that specific public class.

**Answer**: `The source file name must match the class name.`

## Q.19 - What is a constructor's distinguishing feature in Java?

| Prompts                                                          | Answers                                  |
| ---------------------------------------------------------------- | ---------------------------------------- |
| A constructor has the same name as the class and no return type. | Yes, that defines constructors           |
| A constructor must always have parameters.                       | No, constructors can be no-argument.     |
| A constructor can be overridden in subclasses.                   | No, constructors are not inherited.      |
| A constructor is always abstract in design.                      | No, that does not apply to constructors. |
## Q.20 - What type of constructor is created by default if no constructors are defined within a class?


Option B (or Option D, depending on your specific test's exact key definition, as both terms refer to the same default mechanism) is the correct answer.

In standard Java terminology, Option B (No-argument constructor) explicitly describes its structure, while Option D (Default constructor) is the official term for it:

Option D (Default constructor): The official Java terminology for the constructor automatically generated by the compiler when no constructors are explicitly written.

Option B (No-argument constructor): The exact structural form of that default constructor—it takes zero parameters and calls super().

If your quiz treats them as distinct options, Option D is typically the named concept being tested, though Option B precisely describes its syntax.

Why the other options are incorrect:
Option A: The compiler-generated default constructor has public access (if the class is public) or package-private access—never private.

Option C: A parameterized constructor requires explicitly declared parameters, which the compiler will never generate automatically.


**Answer**: `Default constructor`