---
title: Tutorial 4 - SDN150S
date: 2026-03-13 18:38
description:
categories: CPUT
tags:
type: Tutorial
---
### Question 1 

What will be the output of the following C program?
```c
#include <stdio.h>

int main() {
int num = 0;

if (num)
printf("Non-zero");
else
printf("Zero");
return 0;
}
```

```md
zero
```

### Question 2

Match the following control structures to their descriptions:

| Prompt           | Answers                                                                    |
| ---------------- | -------------------------------------------------------------------------- |
| If statement     | Executes an action if the condition is true.                               |
| For loop         | Repeats a block of code a specific number of times.                        |
| While loop       | Repeats a block of code as long as a condition is true.                    |
| Switch statement | Selects one of many blocks of code to execute based on a variable's value. |

### Question 3

Which of the following is an example of an iterative control structure?

- Function
- Switch statement
- While loop
- If statement

```md
While loop
```

### Question 4

What will be the output of the following C program?

```c
#include <stdio.h>

int main() {

  int a = 5, b = 10, c = 15;

if (a < b) {
if (b < c) {
if (a + b > c)
printf("Condition 1\n");
else
printf("Condition 2\n");
} else {

printf("Condition 3\n");
}
 } else {
printf("Condition 4\n");
  }
return 0;
}
```

#### Steps 

Step-by-step:

1️⃣ `a < b`  
5 < 10 → **true**

2️⃣ `b < c`  
10 < 15 → **true**

3️⃣ `a + b > c`  
5 + 10 = 15  
15 > 15 → **false**

So it executes: `printf("Condition 2");`

#### Answer
```md
Condition 2
```

### Question 5

What will be the output of the following C program?

```c
#include <stdio.h>

int main() {

int a = 5, b = 2, c = 7;

if (a <= 0 || b <= 0 || c <= 0) {
 printf("Invalid input\n");
}

else if (a + b <= c || a + c <= b || b + c <= a) {
printf("Not a triangle\n");
}

else if (a == b && b == c) {
printf("Equilateral Triangle\n");
}

else if (a == b || b == c || a == c) {
printf("Isosceles Triangle\n");
}

else {
printf("Scalene Triangle\n");
}

return 0;

}
```

#### Steps 

 int a = 5, b = 2, c = 7;
`(a + b <= c || a + c <= b || b + c <= a`) {

    printf("Not a triangle\n");
#### Answer 
```md
Not a triangle
```

### Question 6

Match the following terms to their corresponding definitions:

| Prompts      | Answers                                                                         |
| ------------ | ------------------------------------------------------------------------------- |
| Input        | Data that is fed into an algorithm.                                             |
| Output       | The result produced by the algorithm.                                           |
| Definiteness | The clarity and unambiguity of the instructions in an algorithm.                |
| Finiteness   | The guarantee that an algorithm will terminate after a limited number of steps. |
### Question 7

In which scenario would you use a switch statement?

```md
When you have multiple possible values for a single variable.
```
### Question 8

An algorithm is a __ procedure to solve a specific problem.

```md
step-by-step
```
### Question 9 

What will be the output of the following C program?

```c
#include <stdio.h>
int main() {

int x = 10;
if (x > 5)

printf("Hello ");
else
printf("World");
return 0;
}
```

```md
Hello
```
### Question 10

What will be the output of the following C program if the user enters the following:

**Enter your choice (1-6): 1**
**Enter temperature value: 100**

```c
#include <stdio.h>

int main() {

int choice;
double temp, convertedTemp;

// Display menu
printf("Temperature Conversion Menu:\n");
printf("1. Celsius to Fahrenheit\n");
printf("2. Fahrenheit to Celsius\n");
printf("3. Celsius to Kelvin\n");
printf("4. Kelvin to Celsius\n");
printf("5. Fahrenheit to Kelvin\n");
printf("6. Kelvin to Fahrenheit\n");
// User input
printf("Enter your choice (1-6): ");
scanf("%d", &choice);
printf("Enter temperature value: ");
scanf("%lf", &temp);

// Switch statement for conversions

switch (choice) {

case 1:
convertedTemp = (temp * 9 / 5) + 32;
printf("Result: %.2lf Fahrenheit\n",convertedTemp);
break;

case 2:
convertedTemp = (temp - 32) * 5 / 9;
printf("Result: %.2lf Celsius\n", convertedTemp);
break;

case 3:
convertedTemp = temp + 273.15;
printf("Result: %.2lf Kelvin\n", convertedTemp);
break;

case 4:
convertedTemp = temp - 273.15;
printf("Result: %.2lf Celsius\n", convertedTemp);
break;

case 5:
convertedTemp = (temp - 32) * 5 / 9 + 273.15;
printf("Result: %.2lf Kelvin\n", convertedTemp);
break;

case 6:
convertedTemp = (temp - 273.15) * 9 / 5 + 32;
printf("Result: %.2lf Fahrenheit\n",convertedTemp);
break;

default:
printf("Invalid choice!\n");
}
return 0;
}
```

```md
Result: 212.00 Fahrenheit
```

### Question 11

What is the default case in a switch statement used for?

when **none of the case values match**.

```md
To handle unexpected values
```

### Question 12

What is the first step in a typical algorithm?

```txt
START
INPUT
PROCESS
OUTPUT
STOP
```

```md
Start
```
### Question 13

Control structures determine the flow of execution in a program.

Examples:

- if  
- switch 
- for
- while

```md
True
```
### Question 14

Pseudocode uses a formal syntax similar to programming languages.

**Pseudocode** is designed to be **informal and easy to read**. It uses plain language to describe the logic of an algorithm without strict programming rules.

```md
False
```
### Question 15

```c
#include <stdio.h>

int main() {

int num = 7;
if (num % 2 == 0)

printf("Even");
else
printf("Odd");
return 0;
}
```

### Question 16

Can we use a switch statement with a floating-point variable?
#### Explain 

No, you cannot use a `switch` statement with a floating-point variable in C.
- The `switch` statement in C only works with **integer-type values**.
Allowed types include:

- `int`
- `char`
- `short`
- `long`
- `enum`
It **does NOT work with**:

- `float`
- `double`

This causes a **compilation error** because `switch` requires an **integer expression**.

>[!NOTE]
>Use **if-else statements** when working with floating-point numbers.

#### Why the other options are wrong

❌ **Yes** → Incorrect because floats cannot be used directly.  
❌ **Only with decimal numbers** → Incorrect; decimals are floats.  
❌ **No** → Not completely correct because conversion makes it possible.
#### Answer
```md
Only if explicitly converted to an integer
```
### Question 17

Which control structure would be best for executing a block of code a specific number of times?
#### Explain
A **for loop** is specifically designed to repeat a block of code **a known number of times**.
#### Why the others are incorrect

❌ **If statement** – Only checks a condition once, no repetition.

❌ **Switch statement** – Used to select between multiple cases, not for repetition.

❌ **While loop** – Repeats while a condition is true, but it is usually used when the number of repetitions is **unknown**.
#### Answer 

```md
For loop
```
### Question 18

The 'default' case in a switch statement is mandatory.
#### Explain 
In C, the **`default` case in a `switch` statement is optional**, not mandatory.

- The `default` case is only used to handle situations where **none of the `case` values match** the variable.
- A program **still compiles and runs**, even though there is **no `default` case**.
#### Answer 

```md
False
```
### Question 19

What will be the output of the following C program?

```c
#include <stdio.h>
int main() {
int p = 4, q = 9, r = 7;

if (p + r > q) {
	if (p * 2 < q) {
		if (r - p < q - r)
			printf("Alpha\n");
		else

 printf("Beta\n");
} else {
printf("Gamma\n");
}

} else {
printf("Delta\n");
}

return 0;

}
```

### Question 20

| Prompts              | Answer                                                               |
| -------------------- | -------------------------------------------------------------------- |
| Bubble sort          | A sorting algorithm that repeatedly steps through the list.          |
| Binary Search        | Searches a sorted array by dividing the search interval in half.     |
| Dijkstra's Algorithm | Finds the shortest path from a source to all other nodes in a graph. |
| Brute Force          | Tries all possible solutions in order to find one that works.        |

