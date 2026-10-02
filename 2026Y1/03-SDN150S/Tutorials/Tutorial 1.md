---
title: Tutorial 1 - SDN150S
date: 2026-02-20 11:45
description:
categories: CPUT
tags:
type: Tutorial
---
## Attempt 1

2026-02-20
### Question 1

Which statement about C standards is accurate based on the material?

```
There are multiple standards, including C89/C90, C99, and C11
```

### Question 2

In the example structure of a C program, what does the function main signify?

```
The entry point of the program
```
### Question 3

What is the purpose of the printf function as used in the examples?

```
To print formatted output to the console
```
### Question 4

Which statement best describes a C identifier?

```
A name used for a variable, function, or other user-defined item
```
### Question 5

Which escape sequence in C moves the output to the next line?

```
\n
```
### Question 6

C is described as a language that teaches what key area important for system programming?

```
Low-level memory management
```
### Question 7

What is the primary purpose of the memory unit description in the content?

```
To store data and programs during processing
```
### Question 8

Write a C program that prints out the phrase:

“**Engineering is an important and learned profession. As members of this profession, engineers are expected to exhibit the highest standards of honesty and integrity**.”

Using single print statements, ensure that each sentence ending with a comma (,) or period (.) is printed on a new line.

```c
#include <stdio.h>

int main(){
printf(“Engineering is an important and learned profession.\n"
 "As members of this profession,\n"
 "engineers are expected to exhibit the highest standards of honesty and integrity.\n”)
 return 0;
}
```

### Question 9

Create two string variables called _firstName_ and _lastName_ respectively. 
Assign the string "**Bob**" to firstName and "**Jones**" to lastName. 
Print _firstName_ and _lastName_ one per newline, using different print statements.

```c
#include <stdio.h>

int main(){
char firstName[] = "Bob";
char lastName[] = "Jones";

printf("First Name: %s\n",firstName);
printf("Last Name: %s\n",lastName);

return 0;
}
```

### Question 10

Variables are containers that can store different data types and values. Declare two string variables that change the age and name of the character in the short story below:

- There once was a man named "**Name**", he was “**Age**” years old. He liked the name "**Name**" but did not like being “**Age**” years old. (Hint: use int for integer, char character string, and print both sentences in separate lines.)

```c
#include <stdio.h>  
  
int main() {  
  
char Name[] = "John";  
int Age = 25;  
  
printf("There once was a man named \"%s\", he was %d years old.\n", Name, Age);  
printf("He liked the name \"%s\" but did not like being %d years old.\n", Name, Age);  
  
return 0;  
}
```

### Question 11

Do the following:

- Create a String variable called "**Name**" and set it to "**Thito**".
- Create an integer variable called "**Age**" and set it to **30**.
- Create an integer variable called "**IQ**" and set it to the value of age.
- Print the Name, Age, and IQ values to console without using a newline.

```c
#include <stdio.h>

int main() {

char Name[] = "Thito";
int Age = 30;
int IQ = Age;

printf("Name: %s Age: %d IQ: %d", Name, Age, IQ);

return 0;
}
```
### Question 12

Write a C program that finds the **area of a triangle** given two integers.

```c
#include <stdio.h>

int main() {

int base, height;
float area;

printf("Enter the base of the triangle: ");
scanf("%d", &base);

printf("Enter the height of the triangle: ");
scanf("%d", &height);

area = 0.5 * base * height;
printf("The area of the triangle is: %.2f", area);

return 0;
}
```
### Question 13

Write a C program that calculates the circumference of a circle, given pi is 3.142.

```c
#include <stdio.h>

int main(){
// Set Variables
const float pi = 3.142f;
float radius,circumference_circle;
// Input Radius
printf("What is the radius?:");
scanf("%f",&radius);
//circumference of a circle
circumference_circle = 2 * pi * radius;
printf("The circumference_circle is: %.2f\n",circumference_circle);
return 0;
}
```
### Question 14

Debug the simple C program below. Look carefully at each line of code and correct the syntax where necessary.

```
1. include<stdio.h>
 
2.
 
2. /* function main begins */
 
3. int_main(void e){
 
5.     printf("Welcome to C! n")
 
4. }
```

```c
#include <stdio.h>
 
int main(void) {
    printf("Welcome to C!\n");
    return 0;
}
```

### Question 15

Write a program that:

- Accepts an integer from the user
- Determines whether the number is even or odd
- Displays the result

```c
#include <stdio.h>

int main() {

int number;

printf("Enter a number: ");
scanf ("%d", &number);

if (number % 2 == 0) {
printf ("%d is an even number.\n", number);

} else {

printf ("%d is an odd number.\n", number);
}
return 0;

}
```