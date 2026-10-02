
```cardlink
url: https://www.youtube.com/watch?v=sdYdnpYn-1o&vl=en
title: "How To Integrate Using U-Substitution"
description: "This calculus video tutorial provides a basic introduction into u-substitution.  It explains how to integrate using u-substitution.  You need to determine wh..."
host: www.youtube.com
favicon: https://www.youtube.com/s/desktop/0084d708/img/favicon_32x32.png
image: https://i.ytimg.com/vi/sdYdnpYn-1o/maxresdefault.jpg
```


# Exercises 

## Ex.1 

> Solve
> [link](https://youtube.com/shorts/mEPZHoXLErI?si=W6XYVCQTMfGpBran)

Evaluating the integral:
$$\int x^5 \sqrt{x^3 - 1} \, dx$$

---

### Step 1: Substitution
Set the term under the cube root to $u$:
$$u = x^3 - 1 \implies x^3 = u + 1$$

Take the derivative of both sides:
$$du = 3x^2 \, dx \implies x^2 \, dx = \frac{1}{3} \, du$$

---

### Step 2: Rewrite & Integrate
Split $x^5$ into $x^3 \cdot x^2$ and substitute $u$ into the integral:
$$
\begin{align*}
\int x^5\sqrt{x^3 - 1} \, dx \\
&=\int (x^3) \sqrt{x^3 - 1} \cdot (x^2 \, dx) \\
&= \frac{1}{3} \int (u + 1) u^{1/3} \, du \\
&= \frac{1}{3} \int \left( u^{4/3} + u^{1/3} \right) \, du \\
&= \frac{1}{3} \left[ \frac{3}{7} u^{7/3} + \frac{3}{4} u^{4/3} \right] + C \\
&= \frac{u^{7/3}}{7} + \frac{u^{4/3}}{4} + C
\end{align*}
$$

---

### Step 3: Final Result
Replace $u$ back with $x^3 - 1$:

> [!success] Solution
> $$\int x^5 \sqrt{x^3 - 1} \, dx = \frac{(x^3 - 1)^{7/3}}{7} + \frac{(x^3 - 1)^{4/3}}{4} + C$$

