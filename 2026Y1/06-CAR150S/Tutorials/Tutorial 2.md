# Question 1 

Why are different levels, capacities, and speeds of memory needed in a memory hierarchy? 
Explain in terms of how the CPU requests data from memory

> [[Memory Hierarchy]]
## Answer

The ideal computer without considering power/energy constraints has infinitely large and fast memory:
- Larger memory makes access times slower
- Faster memory is expensive

The solution to this is memory hierarchy, a set level which each provide different speed and size of storage, providing a balance of speed, size and cost.
- The closer the memory is to the [[CPU - Central Processing Unit|CPU]] the faster and smaller it is , the farther the memory is the larger and slower it is 
> cache -> RAM -> SDD/HDD


# Question 2 

Draw a diagram that highlights the above explanation, i.e., draw a memory hierarchy. The diagram must not indicate speed or capacity values but rather use arrows to show in which direction the speed/capacity increases or decrease

## Answer

![[Pasted image 20261004185544.png]]

# Question 3 

Explain how direct mapped, fully associative, and set associative cache organisations function. The cache and main memory can have any number of blocks, however, cache must be smaller than main memory (for obvious reasons)

## Answer


# Question 10 

List 4 memory technologies.

## Answer 

- Magnetic (incl. HDD)
- optical
- flash (incl. SSD)
- DRAM
- SRAM

# Question 11 

What are two advantages and two disadvantages of flash memory over magnetic storage?

## Answer 

### Advantages

much faster (hundreds of times faster, in theory) and smaller in physical size. It is also less power hungry with less heat dissipation. Finally, it has no moving parts.


### Disadvantages

higher cost per GB and less write operations (after say 100000 writes to a specific bit, this bit will become unreliable, and data can be lost).


# Question 12 

Describe the techniques used to fetch a missing word.

## Answer 

# Question 13 

Explain the types of errors that can occur in memory, and what is done to counteract these errors.
## Answer 



