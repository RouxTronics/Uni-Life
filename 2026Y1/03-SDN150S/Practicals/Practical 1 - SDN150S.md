---
date: 2026-02-25 10:20
categories:
  - CPUT
  - SDN150S
type:
  - Practical
---
## Question 1 
[10 Marks]

- Review the screenshot of the C program shown in Figure 1.
- The program intends to correctly convert hex, octal, and decimal values. 
- However, a student wrote the following C code to perform radix conversion using different numeric bases but encounters an unexpected output.

> [!info]- Given Code
> ```c
> #include <stdio.h>  
> int main(){  
> unsigned int Value = 0xFFFFFFF2; // hexadecimal representation  
> // print conversion to console  
> printf("Decimal: %i\n", Value);  
> printf("Octal: %c\n", Value);  
> printf("Hexadecimal: %d\n", Value);  
> printf("character: %o\n", Value);  
> return 0;  
> }
> 
> /*
> Decimal: -14
> Octal: �
> Hexadecimal: -14
> character: 37777777762
> */
> ```

### 1.1. 

**Explain why the program gives the incorrect result of instead of the correct result.** 
[5 Marks]

The program gives incorrect results because the format specifiers used in the printf(), do not match the data type of the variable and the required output format. 

The variable is declared as: 

unsigned int Value = 0xFFFFFFF2; 

Since Value is an unsigned integer, the decimal value must be positive. 

**Line 5:** 

- The format specifier %i or %d is used for signed integer when running the code will get a negative value of, -14.  
- This is incorrect, because a hexadecimal FFFFFFF2 converted to decimal is 4294967282 
- The correct format specifier is %u. 

**Line 6**:  

- The format specifier %c is used to print a character, not octal value. 
- The correct format specifier is %o 
- Placing a 0 before %o is standard practice so 0%o

**Line 7:**  

- %d is used to print out signed decimal values, negative and positive values, not Hexadecimal. 
- The correct format specifier is %X  
- It is Standard to include prefix use 0x so use 0x%X  

**Line 8:** 

- The correct format specifier %o is used to print out octal values, not a character. 
- The correct format specifier is %c. 
- Also changing character to Character to make all the type of prints start with a capital letter.

### 1.2  
**Re-write the code to ensure the program provides an accurate result. Provide a screenshot of your code and attach the .c file in your practical 1 submission.**
[5 Marks]

```c
/***** AUTHOR INFO ******/
// Name: Etienne Roux
// Student No.:260041637
// Course Title: Sofware Design 1 (SDN150S)
// Date: 26-02-2026

/***** HEADER FILES *****/
#include <stdio.h>

/****** MAIN FUNCTION *****/
int main(){
unsigned int Value= 0xFFFFFFF2; // hexadecimal representation

// print conversion to console
printf("Decimal: %u\n", Value);
printf("Octal: 0%o\n", Value);
printf("Hexadecimal: 0x%X\n", Value);
printf("Character: %c\n", Value);
return 0;
}

/*
Decimal: 4294967282
Octal: 037777777762
Hexadecimal: 0xFFFFFFF2
Character: �
*/
```
## Question 2 
[10 Marks]

- Consider the program shown in Fig. 2 that calculates and prints the number of days in the first half, second half, and the entire current year.
- Notice the initialized variables representing the number of days in each month.
- daysInCurrentFebruary is set to 29, which is typically the number of days in a leap year February. 
- The other months have their standardnumber of days.

> [!info]- Given Code
> ```c
> #include <stdio.h>
> int main(){
> int daysIn CurrentFebrurary = 29;
> int daysIn January = 31;
> int daysIn February = daysInCurrentFebruary;
> int daysIn March = 31;
> int daysIn April = 30;
> int daysIn May = 31;
> int daysIn June = 30;
> int daysIn July = 31;
> int daysIn August = 31;
> int daysIn September = 3*;
> int daysIn October = 3+;
> int daysIn November = 3*;
> int daysIn December = 3+;
> int daysInFirstHalf = daysIn January + daysIn December + daysIn March + daysIn April + daysIn May + daysIn July;
> int daysInSecondHalf = daysIn June + daysIn August + daysIn September + daysIn October + daysIn November + daysIn February;
> printf(“Days in the first half of the current year: %d\n", daysInFirstHalf);
> printf(“Days in the second half of the current year: %d\n", daysInSecondHalf);
> printf(“Days in the current year: %d\n", daysInFirstHalf + daysInSecondHalf);
> return 0;
>  }
> ```

### 2.1 

> [!INFO] EXPECTED OUTPUT 
> - Days in the first half of the current year: 182  
> - Days in the second half of the current year: 184  
> - Days in the current year: 366  

**Review the code to find all possible errors and fix them. Your version of the program must print the same result as the expected output shown above.**

The program gives incorrect results due to syntax errors and incorrect variables, also some of the variables are wrongly placed. 

**Line 2 to Line 5:** 

- In C Programming language variables can’t contain space. 
- The variable daysIn {Month} is written incorrectly.
- Also, in line 2 CurrentFebrurary is misspelled, it will create a different variable then line 5 CurrentFebruary so change it to daysInCurrentFebruary 
- Write the variable as daysIn{Month} like in daysInJanuary or daysInCurrentFebruary 
- This ensures that C recognizes it as a single variable. 

**Line 6 to 11:**  

- The variable daysIn {Month} is written incorrectly, there must be no spaces. 
- Write the variable as daysIn{Month}, change variable to daysInMarch all the way to  daysInAugust 
- This ensures that C recognizes it as a single variable. 

**Line 12 to 15:** 

- The variable daysIn {Month} is written incorrectly, there must be no spaces. 
- Write the variable as daysIn{Month}, change variable to daysInSeptember on Line 12 all the way to  daysInAugust on Line 15. 
   
**Line 16:** 

- Again, the variable daysIn {Month} is written incorrectly, there must be no spaces. 
- Also, daysInDecember and daysInJuly in place in the wrong variable it should be in daysInSecondHalf. 
-  Arrange it in the correct order. 

**Line 17:** 

- Again, the variable daysIn {Month} is written incorrectly, there must be no spaces. 
- Also, daysInJune and daysInFebruary in place in the wrong variable it should be in daysInFirstHalf. 
-  Arrange it in the correct order.


```c
#include <stdio.h>
int main()
{
// Variables: Months of the Year
int daysInCurrentFebruary = 29;
int daysInJanuary = 31;
int daysInFebruary = daysInCurrentFebruary;
int daysInMarch = 31;
int daysInApril = 30;
int daysInMay = 31;
int daysInJune = 30;
int daysInJuly = 31;
int daysInAugust = 31;
int daysInSeptember = 30;
int daysInOctober = 31;
int daysInNovember = 30;
int daysInDecember = 31;
// Variable: First Half of the Year
int daysInFirstHalf = daysInJanuary + daysInFebruary + daysInMarch + daysInApril + daysInMay + daysInJune;
// Variable: Second Half of the Year
int daysInSecondHalf = daysInJuly + daysInAugust + daysInSeptember + daysInOctober + daysInNovember + daysInDecember;

printf("Days in the first half of the current year: %d\n", daysInFirstHalf);

printf("Days in the second half of the current year: %d\n", daysInSecondHalf);

printf("Days in the current year: %d\n", daysInFirstHalf + daysInSecondHalf);
return 0;
 }
```
### 2.2

**Re-write the code to ensure the program computes and prints the sum of the days in all four quarters of the current year as shown below.Provide a screenshot of your code and attach the .c file in your practical 1 submission.**

> [!INFO] EXPECTED OUTPUT 
> - Days in Q1 of the current year: 91    
> - Days in Q2 of the current year: 91   
> - Days in Q3 of the current year: 92
> - Days in Q4 of the current year: 92

```c
/***** AUTHOR INFO ******/
// Name: Etienne Roux
// Student No.:260041637
// Course Title: Sofware Design 1 (SDN150S)
// Date: 26-02-2026

/***** HEADER FILES *****/
#include <stdio.h>

/****** MAIN FUNCTION *****/
int main()
{
// Variables: Months of the Year
int daysInCurrentFebruary = 29;
int daysInJanuary = 31;
int daysInFebruary = daysInCurrentFebruary;
int daysInMarch = 31;
int daysInApril = 30;
int daysInMay = 31;
int daysInJune = 30;
int daysInJuly = 31;
int daysInAugust = 31;
int daysInSeptember = 30;
int daysInOctober = 31;
int daysInNovember = 30;
int daysInDecember = 31;
// Variable: Quarters
int Quarter1 = daysInJanuary + daysInFebruary + daysInMarch;
int Quarter2 = daysInApril + daysInMay + daysInJune;
int Quarter3 = daysInJuly + daysInAugust + daysInSeptember;
int Quarter4 = daysInOctober + daysInNovember + daysInDecember;
// Print Outputs
printf("Days in Q1 of the current year: %d\n", Quarter1);
printf("Days in Q2 of the current year: %d\n", Quarter2);
printf("Days in Q3 of the current year: %d\n", Quarter3);
printf("Days in Q4 of the current year: %d\n", Quarter4);
return 0;
 }
```
## Question 3 

[20 Marks]

### 3.1 

**Write a C program to perform the computation and print the desired result**\
[10 marks]
  
A DC motor is used in an automated conveyor belt system in a manufacturing plant. The  
kinetic energy (𝐾𝐸) of the conveyor belt is determined by the formula:

KE = 0.5 * mass * velocity * velocity

- Where the mass (𝑚) of the conveyor belt is 12.75kg and the velocity (𝑣) of the belt is 3.6 𝑚/𝑠. 
- To improve the performance monitoring, the system needs to compute the kinetic energy as an integer value to be store in a microcontroller.

```c
/***** AUTHOR INFO ******/
// Name: Etienne Roux
// Student No.:260041637
// Course Title: Sofware Design 1 (SDN150S)
// Date: 26-02-2026

/***** HEADER FILES *****/
#include <stdio.h>

/****** MAIN FUNCTION *****/

int main (){
// Variables
float mass = 12.75f;
float velocity = 3.6f;
int kineticEnergy = 0.5 * mass * velocity * velocity;

printf("The value of the mass is: %.2f kg\n", mass);
printf("The value of the velocity is: %.2f m/s\n", velocity);
printf("The value of the kinetic energy, as an integer, is: %d J\n",kineticEnergy);

return 0;
}
```


### 3.2 

**Write a C program that calculates the energy consumed over a given time duration (𝑡)**

A smart power monitoring system is installed in an industrial workshop. 
It operates on a fixed voltage supply of 230V and current of 8.5A to track the energy consumption of a high-power electrical device. 
The system performs real-time calculations based on the power and energy equation given below:

𝑃 = 𝑉 × 𝐼  
𝐸 = 𝑃 × 𝑡

Where 𝑃 denote the Power, 𝐼 denote the current, 𝑉 denote the voltage, 𝐸 denote the energy consumed, and 𝑡 denote the time duration.

Based on the following steps:
• Define voltage as a `#define` preprocessor directive.
• Define current as a const float.
• Compute power using the given formula.
• Convert power to an unsigned int using type casting.
• Accept time duration (𝑡 in hours) as user input.
• Compute energy consumption (E = P × t).
• Convert energy to an unsigned int for efficient storage.
• Display all results using proper format specifiers (%f, %d, %u).

```c
/***** AUTHOR INFO ******/
// Name: Etienne Roux
// Student No.:260041637
// Course Title: Sofware Design 1 (SDN150S)
// Date: 26-02-2026

/***** HEADER FILES *****/
#include <stdio.h>

/****** GLOBAL VARIABLES *****/
#define VOLTAGE 230

/***** MAIN FUNCTION *****/
int main()
{
// Variables
const float current = 8.5f; //current as constant float
float power = VOLTAGE * current; // formula of  power,  P = V × I
unsigned int powerInt = (unsigned int) power; // Type casting of power to unsigned int

// Time duration(hours) from user input
int time;
printf("Enter time duration in hours: ");
scanf("%d", &time);

// Type casting energy
float energy = power * time; // Computing energy using E = P × t
unsigned int energyInt = (unsigned int) energy; // Convert energy to unsigned int

// Prints output the power the results results
printf("\nPower is Calculate  P = V × I\n");
printf("Voltage(V): %d V\n", VOLTAGE);
printf("Current(I): %.2f A\n", current);
printf("Power(P): %.2f W\n", power);

// Prints output the Energy the results results
printf("\nEnergy is Calculate  E = P × t\n");
printf("Power(P): %u W\n", powerInt);
printf("Time Duration(t): %d h\n", time);
printf("Energy(E): %u Wh\n", energyInt);

return 0;
}
```