---
title: Practical 2
date: 2026-03-10 08:46
description:
categories:
  - CPUT
  - SDN150S
tags:
type:
  - Practical
---
## Question 1 

>[!INFO]-
>```c
#include <stdio.h>  
int main(void){  
int xValue = 5;  
int yValue = 9;  
int data;  
int bigData;  
/*  
increment xValue by 3  
decrement yValue by xValue  
multiply xValue times yValue giving data  
increment data by data  
decrement data by 1  
assign data modulo data to yValue  
increment data by data added to xValue  
assign data times data times data to bigData  
increment data by xValue times yValue  
*/  
printf("data: %d\n", data);  
printf("big data: %d\n", bigData);  
return 0;  
 }```


### 1.1.

Re-view the multiline comment and translate it to into an actionable C code. Ensure the program provides an accurate result.

```c
#include <stdio.h>

int main(void){

int xValue = 5;
int yValue = 9;
int data;
int bigData;

/* translated code */

xValue = xValue + 3;
yValue = yValue - xValue;
data = xValue * yValue;
data = data + data;
data = data - 1;
yValue = data % data;
data = data + xValue;
bigData = data * data * data;
data = data + (xValue * yValue);

printf("data: %d\n", data);
printf("big data: %d\n", bigData);

return 0;
}
```
### 1.2. 

Extend the code to obtain the hexadecimal, octal, and ASCII character representation  
of the data value in 1.1. Provide a screenshot of your code and attach the .c file in  
your practical 2 submission.
