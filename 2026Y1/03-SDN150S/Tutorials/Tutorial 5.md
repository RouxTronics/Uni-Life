---
title: Tutorial 5 -SDN150S
date: 2026-03-28 16:12
description:
categories: CPUT
tags:
type: Tutorial
---
## Question 1 

Complete the code that writes a function to print the multiplication table of a given number up to 12.

![](<Tutorial 5 -SDN150S.png>)

### Corrected Code 

```c
#include <stdio.h>

void printTable(int n) {

for (int i = 1; i <=12; i++)
printf("%d x %d = %d\n", n, i,n*i);

}

int main() {
int num;
printf("Enter a number: ");
scanf("%d", &num);
printTable (num);

return 0;
}
```

### Answers 

```
int n
<= 12
i++
n * i
printTable
```

## Question 2 

Match each loop type with its description.

### Mind Trick 

- **for** → “I know how many times” 🔢
- **while** → “Run while true” 🔁
- **do-while** → “Run first, check later” ⚡
- **nested** → “Loop inside a loop” 🧩
### Answer

|Concept|Meaning|
|---|---|
|**For Loop**|Used for a known number of iterations|
|**While Loop**|Executes as long as the condition is true|
|**Do-While Loop**|Executes at least once before checking the condition|
|**Nested Loops**|Loops within another loop|

## Question 3

How can you avoid an infinite loop in a while loop?
### Answer 

By ensuring the condition can eventually evaluate to false.

## Question 4

Debug the code below:
![](<Tutorial 5 -SDN150S-1.png>)

### Corrected Code 

```c
#include <stdio.h>

int main() {
 int choice;
 int count = 0;

  do {
printf("\nMenu:\n");
printf("1. Greet\n");
printf("2. Show Current Count\n");
printf("3. Exit\n");
printf("Enter your choice: ");

scanf("%d", &choice);
	count++; // count how many times menu has been shown
    
switch (choice) {
          case 1:   
            printf("Hello, User!\n");
            break;
    
          case 2:
            printf("The menu has been shown %d times.\n", count );
			break;
   
		    case
    
    :
    
            printf("Exiting program...\n");
    
            break;
    
    :
    
            printf("Invalid choice. Please try again.\n");
    
        }
    
      } while (choice 3);  
return 0;
}
```

### Answers 

```
%d
&
choice
1
2
count
break
3
default
==
```

## Question 5

Write a function to print the Fibonacci series up to n terms.

![](<Tutorial 5 -SDN150S-2.png>)

### Corrected Code 

```c
#include <stdio.h>

void printFibonacci(int n){
	int a = 0,b=1,c;
	
	for(int i=0;i<n;i++){
		printf("%d",a);
		c = a+b;
		a =b;
		b=c;
	}
}

int main(){
	
	int terms;
	printf("Enter number of terms: ");
	scanf("%d",&terms);
	printFibonacci(terms);
	
	return 0;
}
```

### Answer 

```
int
i<n
i++
&terms
terms
```
## Question 6 

A while loop can lead to an infinite loop if its condition is always true.

### Answer 

True

## Question 7

Write a C program that asks the user for the number of rows, and prints a number pyramid using nested for loops.

![200](<Tutorial 5 -SDN150S-3.png>)
### Corrected Code 

```C
#include <stdio.h>

int main() {

int rows;

printf("Enter number of rows: ");
scanf("%d", &rows);

for (int i = 1; i <= rows; i++) {

// print spaces
for (int j = 1; j <= rows - i; j++) {
printf(" ");
}

// print numbers
for (int k = 1; k <= i; k++) {
	printf("%d ", k);
}

printf("\n");
  }
  return 0;
}
```

## Question 8

Write a function to reverse an integer using a loop. (e.g., Input: 1234 → Output: 4321)

### Corrected Code 

```c
#include <stdio.h>
int reverseNumber(int n) {
	int reversed = 0;

	  while (n > 0) {
	    reversed = reversed * 10 + (n % 10);
	     n /= 10;
	 }
 return reversed;
}

int main() {

  int num;
	printf("Enter a number: ");
	scanf("%d", &num);
	printf("Reversed Number = %d\n", reverseNumber(num));

  return 0;
}
```

## Question 9
Write a C program using a **while loop** to calculate the sum of all natural numbers from 1 to n, where n is entered by the user.

```c
  
#include <stdio.h>

  

int main() {

  int n, i = 1, sum = 0;

  

  printf("Enter a positive integer: ");

  scanf("%d", &n);

  

  while (i <= n) {

    sum += i;

    i++;

  }


  printf("Sum of first %d natural numbers is %d\n", n, sum);

  return 0;

}
```
## Question 10

In C programming, a __ loop is typically used when the number of iterations is known beforehand.

### Explain

- `for` loop → used when you **know how many times** to repeat
- `while` loop → used when repetitions depend on a **condition**
### Answer 

```
for
```

## Question 11

What is the primary benefit of using functions in programming?

### Explain 

```c
void greet() {
    printf("Hello\n");
}
greet();
greet();
```
### Answer 

```
Code reusability and modular design.
```
## Question 12

Which statement correctly describes the syntax of a function definition in C?
### Explain 

```c
return_type function_name(parameters) {
    // body of the function
}

int add(int a, int b) {
    return a + b;
}
```

### ❌ Why the other options are wrong

- **“It must contain at least two parameters.”**  
    ❌ False — functions can have **zero, one, or many** parameters
- **“It must start with a for loop declaration.”**  
    ❌ No — loops are optional inside functions
- **“It does not require a return type.”**  
    ❌ Wrong — every function **must have a return type** (`int`, `void`, etc.)
### Answer 
```
It includes a return type, function name, and parameter list.
```
## Question 13

### Quick Memory Tricks

- **Local** → “only here” 📍
- **Global** → “everywhere” 🌍
- **Declaration** → “telling the compiler” 🗣️
- **Call** → “run the function” ▶️
### Answer 

| Concept                  | Meaning                                                                |
| ------------------------ | ---------------------------------------------------------------------- |
| **Local Variable**       | Accessible only within a specific function                             |
| **Global Variable**      | Accessible throughout the entire program                               |
| **Function Declaration** | A statement that tells the compiler the function's name and parameters |
| **Function Call**        | The process of invoking a defined function                             |
## Question 14

Write a function that checks whether a given number is a **palindrome** (i.e., it reads the same backward and forward).

```c
#include <stdio.h>
int isPalindrome(int n);

int main() {
  int num;
  printf("Enter a number: ");
  scanf("%d", &num);
  if (isPalindrome(num))
    printf("%d is a palindrome.\n", num);
  else
    printf("%d is not a palindrome.\n", num);

  return 0;
}

int isPalindrome(int n) {
	int original = n, reversed = 0;
  
  while (n > 0) {
    reversed = reversed * 10 + n % 10;
    n /= 10;
  }
  return original == reversed;
}
```

**Blanks filled:**

- Return type and parameter: `int isPalindrome(int n)`
- `while (n > 0)`
- `n /= 10;`
- `return original == reversed;`
- `isPalindrome(num)`, and both `printf` format specifier/argument: `%d`, `num`
## Question 15

```c
#include <stdio.h>

void decimalToBinary(int n) {
	
	  int binary[8]; // to store 8 bit binary number
	  int i = 0;
	
	if (n == 0) {
	    printf("0");
	    return;
	  }
	
	  while (n > 0) {
	    binary[i] = n % 2;
	    n = n / 2;
	    i++;
	  }
	
	printf("Binary: ");
	  
	  for (int j = i - 1; j >= 0; j--)
	    printf("%d", binary[j]);
	
	 printf("\n");
}

int main() {
  int num;

  printf("Enter a decimal number: ");
  scanf("%d", &num);

  decimalToBinary(num);

  return 0;
}
```

**Blanks filled:**

- Return type and parameter: `void decimalToBinary(int n)`
- Array declaration: `int binary[8];`
- `binary[i] = n % 2;`
- For loop condition and increment: `j >= 0; j--`
- Array access in print: `binary[j]`
- `scanf("%d", &num);`
- `decimalToBinary(num);`

## Question 16
Write a program with a function that counts even and odd numbers from 1 to n.
### Corrected Code 

```c
#include <stdio.h>

void countEvenOdd(int n) {

  int even = 0, odd = 0;

  for (int i = 1; i <= n; i++) {

    if (i % 2 == 0)
      even++;
    else
      odd++;
  }

  printf("Even: %d, Odd: %d\n", even, odd);

}

int main() {
  int num;
  printf("Enter a limit: ");
  scanf("%d", &num);
  countEvenOdd(num);
  return 0;
}
```
## Question 17

In a nested loop, when an inner loop completes its run, what happens next?

### Answer 

```
The control returns to the next iteration of the outer loop.
```

## Question 18 

Match the control statement to its functionality.

### 🧠 Quick Memory Trick

- **break** → “STOP the loop” 🛑
- **continue** → “SKIP this round” ⏭️
- **return** → “EXIT function” 🔙
- **goto** → “JUMP somewhere” 🏃
### Answer 

| Prompts  | Answer                                          |
| -------- | ----------------------------------------------- |
| Break    | Exits the loop immediately                      |
| Continue | Skips the current iteration                     |
| Return   | Exits a function and optionally returns a value |
| Goto     | Transfers control to a labeled statement        |

## Question 19 

What will happen if a break statement is used in a loop?

### Explain 

| Statement  | What it does                               |
| ---------- | ------------------------------------------ |
| `break`    | ❌ Stops the loop completely                |
| `continue` | 🔁 Skips current iteration, continues loop |
### Answer 

```
The loop terminates immediately.
```

## Question 20

Match each loop related term to its relevant concept.

| Prompt    | Answer                                 |
| --------- | -------------------------------------- |
| Condition | Determines loop execution.             |
| Iteration | One complete cycle of the loop.        |
| Scope     | Region where a variable is accessible. |
| Syntax    | The rules governing code structure.    |
