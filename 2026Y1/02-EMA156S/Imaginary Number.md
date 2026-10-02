# Understanding the Imaginary Unit $i$

An imaginary number is a real number multiplied by the imaginary unit $i$. It extends the real number system $\mathbb{R}$ to the complex number system $\mathbb{C}$, allowing us to solve equations that have no real-number solutions (such as $x^2 + 1 = 0$).

---

## Key Definitions

* **Fundamental Property:**
  $$i = \sqrt{-1}$$

* **Square of $i$:**
  $$i^2 = -1$$

---

## The Cyclic Pattern of $i$

Multiplying by $i$ represents a **90-degree counterclockwise rotation** on the complex plane. Because four full $90^\circ$ rotations complete a $360^\circ$ circle, raising $i$ to successive positive integer powers creates a repeating 4-step cycle:

| Power | Simplification | Value |
| :--- | :--- | :--- |
| $i^1$ | $i$ | $i$ |
| $i^2$ | $(\sqrt{-1})^2$ | **$-1$** |
| $i^3$ | $i^2 \cdot i = (-1) \cdot i$ | **$-i$** |
| $i^4$ | $i^2 \cdot i^2 = (-1) \cdot (-1)$ | **$1$** |

> [!tip] Quick Evaluation
> To evaluate any high power of $i$ (e.g., $i^{99}$), divide the exponent by $4$ and check the remainder:
> * **Remainder 1** $\rightarrow i$
> * **Remainder 2** $\rightarrow -1$
> * **Remainder 3** $\rightarrow -i$
> * **Remainder 0** $\rightarrow 1$

---

# Exercises

### Q.1 
> Evaluate $i^{87}$
#### Solution

1. Divide the exponent $87$ by $4$ to find the remainder:
   $$87 \div 4 = 21 \text{ with a remainder of } 3$$

2. Rewrite the expression using exponent rules:
   $$i^{87} = (i^4)^{21} \cdot i^3$$

3. Substitute $i^4 = 1$:
   $$i^{87} = (1)^{21} \cdot i^3 = 1 \cdot i^3 = i^3$$

4. Use the cycle table to evaluate $i^3$:
   $$i^3 = -i$$

> [!success]- Answer
> $$-i$$

