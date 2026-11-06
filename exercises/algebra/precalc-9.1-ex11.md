---
source: PRECALC
ref: "9.1 #11"
topics: [system-of-equations, substitution]
difficulty: intro
---

# Substitution

## Problem

Solve by substitution:

$$
\begin{cases}
x + 3y = 5 \\
2x + 3y = 4
\end{cases}
$$

## My attempt

**Solve the first equation for $y$:**

$$
\begin{aligned}
x + 3y &= 5 \\
3y &= 5 - x \\[6pt]
y &= \frac{5 - x}{3}
\end{aligned}
$$

**Substitute into the second equation to find $x$:**

$$
\begin{aligned}
2x + 3\left(\frac{5 - x}{3}\right) &= 4 \\[6pt]
2x + (5 - x) &= 4 \quad \left(\tfrac{3}{3} = 1\right) \\
x + 5 &= 4 \\
x &= -1
\end{aligned}
$$

**Substitute $x$ back into the first equation to find $y$:**

$$
\begin{aligned}
-1 + 3y &= 5 \\
3y &= 6 \\
y &= 2
\end{aligned}
$$

**Check in both original equations.**

- $-1 + 3(2) = -1 + 6 = 5$ ✓
- $2(-1) + 3(2) = -2 + 6 = 4$ ✓

**Answer.** $(-1,\ 2)$

## Mistake / lesson

- **Isolate the variable with coefficient $\pm 1$.** In $x + 3y = 5$, isolating $x$ gives
  $x = 5 - 3y$ with no fractions. Isolating $y$ created $\frac{5 - x}{3}$, which only worked out
  because the 3 cancelled later. (Same idea as [ex12](precalc-9.1-ex12.md).)
- **Cancel before distributing.** In $3 \cdot \frac{5 - x}{3}$ the 3s cancel immediately, leaving
  $5 - x$. Distributing first and then dividing is an extra step and an extra chance for error.

## Related

- [Systems of linear equations](../../notes/algebra/systems-of-linear-equations.md)
