---
title: Tutorial 3 - SDN150S
date: 2026-03-09 19:18
description:
categories:
  - CPUT
  - SDN150S
tags:
type:
  - Tutorial
---
## Question 1 


| storage Class |                                         |
| ------------- | --------------------------------------- |
| auto          | Local variable with garbage value.      |
| static        | Retains value across function calls     |
| extern        | Used for access across multiple files   |
| register      | Stored in CPU registers for fast access |

## Question 2 

What will be the output of the program above?

```c
#include <stdio.h>

int main() {

int a = 25, b = 8;
printf("%d%d\n", a ^ b, a | b);

return 0;
}
```

### Explain 

```md 
Binary:
25 = 11001
8  = 01000

XOR (^)
11001
01000
-----
10001 = 17

OR (|)
11001
01000
-----
11001 = 25
```
### Answer
```md
1725
```

## Question 3 

| Operator            | Answers                                         |
| ------------------- | ----------------------------------------------- |
| Arithmetic Operator | Performs mathematical calculations on operands. |
| Relational Operator | Compares two values and returns true or false.  |
| Bitwise Operator    | Performs operations on bits of integers.        |
| Logical Operator    | Combines multiple boolean expressions.          |
## Question 4

All C operators have the same level of recedence regardless of their types.

**Operators have different precedence levels.**

```md
False
```

## Question 5

What will happen if you attempt to retrieve the address of a register variable in C?
### Explain 

Register variables are stored in **CPU registers**, not memory.

You **cannot use `&`** to get the address.
### Answer 
```md
It will result in a compilation error
```
## Question 6

The __ storage class retains a variable's value between function calls, enabling it to maintain state.

```md
static
```

## Question 7

In C, the __ storage class is used for local variables and has a scope limited to the block they are defined in, often initialized to garbage value if not specified.

```md
```

## Question 8

To enhance performance by storing variables in the CPU, the __ storage class is used, although it cannot be accessed by the address operator.

```md
register
```

## Question 9

A = 10
B = 2

What will the bitwise operation of **(A >> B)** be in decimal?
### Example 

```md
A = 10  
B = 2  
A >> B

Right shift by 2.

10 = 1010  
1010 >> 2 = 0010
```
### Answer 

```md
2
```

## Question 10

The static storage class allows variables to retain their value even after the function has finished executing.

Static variables **retain their value after function ends**.

```md
True
```

## Question 11

```c
#include <stdio.h>
int main() {

int x = 5, y = 10;

(x > y) ? (x = x + 5) : (y = y + 5);
printf ("x = %d, y = %d\n", x, y);

return 0;

}
```

```md
x = 5, y = 15
```

## Question 12

M = 0000 1111
N = 0000 0100

What will the bitwise operation of (M << N) be in decimal?

### Explain 

```md
M = 00001111 = 15
N = 00000100 = 4

M << N  
15 << 4

Left shift 4:
00001111 → 11110000
```

### Answer 

```md
240
```
## Question 13

```c
#include <stdio.h>
int main() {
int x = 10;

  x += 5 * 2;
  printf("%d\n", x);

  return 0;
}
```
### Example

```md
x = 10  
x += 5 * 2

Operator precedence:
5 * 2 = 10

Then
x = 10 + 10
x = 20
```
### Answer
```md
20
```

## Question 14
`
```c
#include <stdio.h>
int main() {

int a = 5, b = 10;
int x = a++ + b; 
int y = ++a + b; 

printf("x = %d, y = %d, a = %d\n", x, y, a);
return 0;
}
```

### Example 

```c
int a = 5, b = 10;  
int x = a++ + b;  
int y = ++a + b;
```

Step by step:
First line
x = a++ + b

Post increment → use **5 first**
`x = 5 + 10 = 15  `
a becomes 6

Second line
`y = ++a + b`
Pre increment → increase first

```
a = 7  
y = 7 + 10 = 17
```
### Answer 

```md
x = 15, y = 17, a = 7
```
## Question 15

In C, the operator that returns the size of a type or variable is called __

```md
sizeof
```
## Question 16

Which of the following is not a storage class in C?
```md
dynamic
```
## Question 17

```c
#include <stdio.h>

int main() {

int x = 10, y = 3;
float result = (float)x /y; 

printf("Result: %f\n", result);

return 0;
}
```

What will be the output of the program above?
**type casting to float**.

```md
Result: 3.333333
```
## Question 18

x = 0001 1011
y = 1011 0001

What will the bitwise operation of **(x & y)** be in decimal?
### Explain 

x = 00011011 = 27  
y = 10110001 = 177

```
Bitwise AND:

00011011  
10110001  
--------  
00010001
```

Decimal: 17

### Answer 

```md 
17
```
## Question 19

The extern storage class can be used to access global variables defined in other files.

Extern can access **global variables from other files**.

```md 
True
```

## Question 20
What will be the output of the statement `printf("%d", 5 + 10 * 2);`?

### Explain 

```md
10 * 2 = 20
5 + 20 = 25
```

### Answer 

```md
25
```