---
title: Chapter 5 -SDN150S
date: 2026-03-29 08:06
description:
categories: CPUT
type: Lecture
course: SDN150S
tags:
  - c
---
# Examples 

## 5.1 

```c
#include <stdio.h>
#include <stdint.h>

int main(){
uint8_t i =0;
while(1){
printf("%d\n",i);
i++;
}
retrun 0;
}
```

## 5.2 

```c
#include <stdio.h>
#include <stdint.h>

int main(){
uint8_t i =0;
while(i<5){
printf("%d\n",i);
i++;
}
retrun 0;
}
```

## 5.3 

```c
#include <stdio.h>
#include <stdint.h>
#include <stdbool.h>

int main(){
uint8_t i =0;
while(true){
	if(i>10){
	break;
	}
printf("%d\n",i);
i++;
}
retrun 0;
}
```

## 5.4 

```c
#include <stdio.h>
#include <stdint.h>

int main(){
uint8_t i =0;
for (i = 0; i<10;i++){
	printf("%d\n",i);

}
retrun 0;
}
```

## 5.5 

```c
#include <stdio.h>
#include <stdint.h>
#includ <stdbool.h>

int main(){
uint8_t i =0;
for (i = 0; i<10;i++){
	printf("%d\n",i);

}
retrun 0;
}
```