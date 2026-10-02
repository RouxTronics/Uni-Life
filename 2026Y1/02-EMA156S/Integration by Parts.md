# Rule
$$ \intop udv = uv - \intop v du$$

> LIATE
- L:
- I:
- A:
- T:
- E: 

---
# Exercises 

## Ex.1

$$\intop 3x\sec x\tan x \space dx$$
### Step 1: Setup Integration by Parts
Factor out the constant and assign variables:
$$3 \int x \sec x \tan x \, dx$$

* $u = x \implies du = dx$
* $dv = \sec x \tan x \, dx \implies v = \sec x$

### Step 2: Evaluate

$$
\begin{align*}
3 \int x \sec x \tan x \, dx &= 3 \left( x \sec x - \int \sec x \, dx \right) \\
&= 3x \sec x - 3 \ln |\sec x + \tan x| + C
\end{align*}
$$

### Solution
> [!success]
> $$ 3x \sec x - 3 \ln |\sec x + \tan x| + C$$

