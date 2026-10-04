# Overview 
Amdahl's law is a computer science formula that **calculates the maximum theoretical speedup of a task when only a portion of that task is improved or run in parallel**

- **Origin:** Computer architect **Gene Amdahl** introduced the principle in **1967**.

- **The ceiling:** Even with an infinite number of processors, the total speedup is strictly limited by the time spent on the part that cannot be sped up

- Diminishing returns:  Adding more computer processors helps up to a point, but the unchangeable sequential (non-parallel) part of the task holds back further gains.
## Formula 
![[Pasted image 20261002220230.png]]

![[Pasted image 20261002220300.png]]

$$S = \frac{1}{(1-P)+ \frac{P}{N}}$$


- S ($Speed_{{overall}}$)= calculates the maximum theoretical speedup of a task when only a portion of that task is improved or run in parallel

- P ($fraction_{{enhanced}})$ = The fraction of the task or program that can be parallelized or improved

- N ($Speedup_{enhanced}$) =  The number of processors or cores added to the system.
## Resources 

- [Wikipedia source ](https://en.wikipedia.org/wiki/Amdahl%27s_law)
- [Amdahl's law in Computer Organization](https://www.geeksforgeeks.org/computer-organization-architecture/computer-organization-amdahls-law-and-its-proof/) -Geeksforgeeks

---
# Problems

## Problem 1 

A central processing unit designed with a neural network accelerator can perform a face identification 246% faster than without the accelerator when doing certain security functions (e.g., unlocking a phone using the camera).

What percentage of face identification operations are required to achieve an overall speedup of 2? Assume that the face identification is the time in the original execution spent on security functions. 

### Solution 
*Given:*
- $N: speed_{enchanced} =2.46$
- $S =2$

![[Pasted image 20261002224241.png]]

$Fraction_{{enchanced}} =0.842$

## Problem 2 

![[Pasted image 20261002224906.png]]

