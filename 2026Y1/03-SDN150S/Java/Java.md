# Overview 

Java is an [Object-Oriented Programming](https://en.wikipedia.org/wiki/Object-oriented_programming) language 
Created [James Gosling](https://en.wikipedia.org/wiki/James_Gosling) by in 1995, released by Sun Microsystems

It makes use of:
- objects: 
- classes: 

In Java, identifier naming rules state that:

- Identifiers **cannot start with a digit** (0–9).
    
- Identifiers can begin with a letter (A–Z or a–z), a currency symbol (e.g., `$`), or an underscore (`_`).
    
- Subsequent characters can include digits, letters, `$`, or `_`.

---
# Usage 
> [Cheatsheet](https://cheatsheets.zip/java)
## How to Print hello world in Java

```java
public class Main{
	public static void main(String[] args){
		System.out.println("Hello-World");
	}
}
```

## User input - Name & age

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        // Prompt user and read String input
        System.out.print("Enter name: ");
        String myName = input.nextLine();

        // Prompt user and read integer input
        System.out.print("Enter number: ");
        int myNum = input.nextInt();

        // Display results
        System.out.println(myNum);
        System.out.println(myName);
        
    }
}
```

## Creating an for loop 

```
for (initialization; loopContinuationCondition; increment) {
    // statement(s) to execute repeatedly
}
```

```java 
public class ForLoopExample {
    public static void main(String[] args) {
        for (int count = 1; count <= 10; count++) {
            System.out.printf("%d ", count);
        }
    }
}
```

---
# Resources 
- Tutorials: 10-13
- How to Program Java,10e (2015) - Paul Deitel, Harvey Deitel