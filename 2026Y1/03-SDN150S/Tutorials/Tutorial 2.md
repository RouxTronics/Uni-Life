---
title: Tutorial 2
date: 2026-02-28 09:08
description:
categories:
  - CPUT
  - SDN150S
type:
  - Tutorial
tags:
  - cput/sdn150s
---
### Question 1

The sizeof operator can return varying sizes for the same data type on different systems.

Different systems (32-bit vs 64-bit) may store data types in different sizes.  
Example:

- `int` → 4 bytes (most systems)
- `long` → 4 bytes (Windows 64-bit) or 8 bytes (Linux 64-bit)

```md
True
```


### Question 2 

A mathematician needs a program to calculate the area of a rectangle and a circle using macros.

Write a C program that:

1. Uses `#define` to declare macros for calculating the area of a rectangle and a circle.
2. in the main function, computes the area of:
	- A rectangle with **length = 10** and **width = 5**
	- A circle with **radius = 7**
3. Prints the computed results.

```c
#include <stdio.h>
#define PI 3.14
#define AREA_CIRCLE (PI * radius * radius)
#define AREA_RECTANGLE (length * width)

int main(){
    int length = 10;
    int width = 5;
    int radius = 7;
    
	printf("The Area of the Circle is: %.2f\n", AREA_CIRCLE); 
	printf("The Area of the Rectangle is: %d\n", AREA_RECTANGLE); 
    return 0;
}

```

### Quesiton 3 

Enumerated types in C are automatically assigned integer values starting from zero.

Example:

```c
enum Day {MON, TUE, WED};
```

- MON = 0
- TUE = 1
- WED = 2

```md
True
```
### Question 4 

A programmer wants to convert a given uppercase character to lowercase using ASCII values. Write a C program that reads an uppercase letter from the user, converts it to lowercase using ASCII values, and prints the result.

```c
#include <stdio.h>

int main(){

    char uppercase;
    char lowercase;
   printf("What uppercase letter would you like to input? ");
   scanf("%c",&uppercase);
   
   lowercase = uppercase +32;
   printf("\nThe lowercase of that letter is: %c\n", lowercase);

   return 0;  
}
```

### Question 5

The __ is used to determine the size in bytes of a data type or variable in C.

```md
sizeof
```

### Question 6

Match the following data types with their descriptions:

| data_types | descriptions                                            |
| ---------- | ------------------------------------------------------- |
| int        | Store Whole numbers                                     |
| float      | Stores decimal numbers(single precision)                |
| strut      | User-defined data type that groups different data types |
| char       | store single character                                  |
### Question 7

Macros defined with `#define `can only be used with integer values.

Macros can be used with:

- Integers 
- Floats
- Expressions
- Code blocks
Example:

```c
#define PI 3.14159
```

```md
False
```
### Question 8

What is the output of the sizeof operator when used on a float variable?

```md
Typically returns 4 bytes.
```

### Question 9

In C programming, a __ is a symbolic name representing a memory location where data is stored. 

```md
variable
```
### Question 10

Explain the significance of the sizeof operator in C programming.

**The sizeof operator is used to determine the size of an data type in bytes.**
for example using  the data type float.
the value of PI is 3.14, but the size of the float is 4 bytes.

```c
#include <stdio.h>

int main(){
float PI = 3.1412;
printf("PI is equal to %.2f\n",PI);
printf("The size of PI is: %d\n", sizeof(PI));

return 0;
}
```
### Question 11

What are the main differences between primitive data types and derived data types in C?

The main difference is the way they store data.
- **primitive data types** store only one value at a time, it uses data types like float, int and char.
- **derived data types** stores multiple values at a time like arrays and structures
### Question 12

You cannot modify a variable once it has been declared in C.

```c
False
```
### Question 13

A software engineer is designing a program to store a student's details, including their ID (integer), GPA (floating-point number), and a grade (character). Write a C program that declares and initializes these variables, then prints their values.

```c
#include <stdio.h>

int main(){
 // Variables
    unsigned int idNumber; // Student ID number
    float gpaValue; // Students GPA value
    char grade; // The grade they got
    
    /***** User Inputs *****/ 
   
    // Student ID
    printf("Input student ID Number: ");
    scanf("%u", &idNumber);
    // GPA
    printf("Input student GPA: ");
    scanf("%f", &gpaValue);
    //Grade
    printf("Input student Grade: ");
    scanf(" %c", &grade);
    
    // Print Outputs 
    printf("Student ID: %u\n", idNumber);
    printf("GPA: %.2f\n", gpaValue );
    printf("Grade: %c\n", grade);
    
    return 0;
}
```
### Question 14 

What is the purpose of the void data type in C?

It indicates no value is available.: void 

```md
void
```
### Question 15 

In C, the basic building blocks of data manipulation are known as __ 

```md
variables
```

### Question 16 

What does the keyword 'const' indicate when declared with a variable?

```md
The variable's value cannot be changed after its initialization.
```

### Question 17

Match the following identifiers with their meanings:

| Identifier    | Meaning                                     |
| ------------- | ------------------------------------------- |
| **const**     | A keyword to define a constant value        |
| **typedef**   | Used to create new data type names          |
| **enum**      | A keyword to define enumerated data types   |
| **struct**    | Used to define a structure                  |
| **`#define`** | Used to define symbolic constants or macros |


### Question 18

Match the terms related to data types with their characteristics:

| data types          | characteristics                                         |
| ------------------- | ------------------------------------------------------- |
| primitive data type | Basic types built into C like int and char.             |
| derived data type   | Types formed from primitive types such as arrays.       |
| enumeration         | A user-defined type with a set of named constants.      |
| size                | Determines the memory storage required for a data type. |
