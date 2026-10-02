
---

## What is C?

C is a general-purpose, mid-level programming language originally developed for building the UNIX operating system. It gives direct access to hardware and memory, making it the language of choice for operating systems, embedded systems, compilers, databases, and game engines — anywhere efficiency and portability matter.

## Why use C?

> [!info]- Reasons to learn C
> 
> - **Performance** — compiles to native machine code with minimal overhead
> - **Portability** — runs on virtually every platform and architecture
> - **Control** — direct memory management via pointers and manual allocation
> - **Foundation** — C++, C#, Java, Python, and Go are all influenced by C syntax
> - **Ubiquity** — Linux kernel, CPython interpreter, SQLite, and most firmware are written in C

---

## How to use C

```cardlink
url: https://cheatsheets.zip/c
title: "C Cheat Sheet & Quick Reference"
description: "C quick reference cheat sheet that provides basic syntax and methods."
host: cheatsheets.zip
favicon: https://cheatsheets.zip/images/favicon.png?v=1
image: https://cheatsheets.zip/assets/image/c-preview.png?v=ybhmo
```


> [!tip] Cheat Sheet [C Cheat Sheet & Quick Reference](https://cheatsheets.zip/c) — syntax and methods at a glance

### Hello World

**1. Create the file**

```bash
nano hello_world.c
```

**2. Write the program**

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

**3. Compile and run**

```bash
gcc hello_world.c -o hello_world
./hello_world
```

---

## Topics

### Control Flow

#### For loop

```c
for (int i = 0; i < 10; i++) {
    printf("Hello\n");
}
```

#### While loop

```c
int i = 0;
while (i < 10) {
    printf("Hello\n");
    i++;
}
```

#### If / else

```c
if (x > 0) {
    printf("Positive\n");
} else if (x < 0) {
    printf("Negative\n");
} else {
    printf("Zero\n");
}
```

### Data Types

|Type|Size|Example|
|---|---|---|
|`int`|4 bytes|`int x = 5;`|
|`float`|4 bytes|`float f = 3.14;`|
|`double`|8 bytes|`double d = 3.14159;`|
|`char`|1 byte|`char c = 'A';`|
|`char[]`|n bytes|`char s[] = "hello";`|

### Strings
> Strings

```c
#include <stdio.h>
#include <string.h>

int main() {
    char name[] = "Rouxtronics";

    printf("Name:   %s\n",  name);
    printf("Length: %lu\n", strlen(name));

    // Copy
    char copy[50];
    strcpy(copy, name);

    // Concatenate
    char greeting[50] = "Hello, ";
    strcat(greeting, name);
    printf("%s\n", greeting);

    return 0;
}
```

### Pointers

> [!example] See dedicated note Pointers

```c
int x = 10;
int *ptr = &x;       // ptr holds the address of x

printf("%d\n", *ptr); // dereference — prints 10
*ptr = 20;            // modifies x through the pointer
printf("%d\n", x);    // prints 20
```

### Functions

```c
#include <stdio.h>

int add(int a, int b) {
    return a + b;
}

int main() {
    int result = add(3, 4);
    printf("Result: %d\n", result);
    return 0;
}
```

### Memory Management

```c
#include <stdlib.h>

int *arr = malloc(10 * sizeof(int));  // allocate
if (arr == NULL) { /* handle failure */ }

arr[0] = 42;

free(arr);  // always free what you malloc
arr = NULL;
```

> [!warning] Memory leaks Every `malloc()` or `calloc()` must have a matching `free()`. Forgetting to free is undefined behaviour and a common source of vulnerabilities.

---

## C in Cybersecurity

> [!danger]- Why C matters in security
> 
> - **Buffer overflows** — C has no bounds checking; the basis of many CVEs
> - **Format string attacks** — misuse of `printf()` family
> - **Use-after-free** — freeing memory then accessing it
> - **Shellcode** — most shellcode is written or compiled from C
> - **Kernel exploits** — Linux kernel (C) is a common target
> - **Reverse engineering** — compiled C is what you encounter in binary challenges

---

