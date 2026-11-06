---
source: PRECALC
ref: "9.1 #12"
topics: [system-of-equations, substitution]
difficulty: intermediate
---

# Substitution (simplify first)

## Problem

Solve by substitution:

$$
\begin{cases}
3x - 2y = 18 \\
5x + 10y = -10
\end{cases}
$$

## My attempt

**Solve the first equation for $y$:**

$$
\begin{aligned}
3x - 2y &= 18 \\
-2y &= 18 - 3x \\[6pt]
y &= \frac{18 - 3x}{-2} = \frac{3x - 18}{2}
\end{aligned}
$$

**Substitute into the second equation to find $x$:**

$$
\begin{aligned}
5x + 10\left(\frac{3x - 18}{2}\right) &= -10 \\[6pt]
5x + 5(3x - 18) &= -10 \quad \left(\tfrac{10}{2} = 5\right) \\[6pt]
5x + 15x - 90 &= -10 \\
20x &= -10 + 90 \\
20x &= 80 \\
x &= 4
\end{aligned}
$$

**Substitute $x$ back into the first equation to find $y$:**

$$
\begin{aligned}
3(4) - 2y &= 18 \\
12 - 2y &= 18 \\
-2y &= 6 \\
y &= -3
\end{aligned}
$$

**Check in both original equations.**

- $3(4) - 2(-3) = 12 + 6 = 18$ ✓
- $5(4) + 10(-3) = 20 - 30 = -10$ ✓

**Answer.** $(4,\ -3)$

## Mistake / lesson

- **A negative denominator flips the sign of the whole numerator.** I wrote
  $\frac{-3x + 18}{-2} = \frac{-3x + 18}{2}$, which is wrong. Moving the $-1$ up changes **every**
  term: $\frac{-3x + 18}{-2} = \frac{3x - 18}{2}$. It didn't affect the result only because the next
  step used the previous (correct) line.
- **Simplify first, then choose what to isolate.** The second equation divides by 5:
  $x + 2y = -2$, so $x = -2 - 2y$ with no fractions at all. Before isolating, look for an equation
  that can be simplified or a variable with coefficient $\pm 1$.

## Related

- [Systems of linear equations](../../../notes/algebra/linear-systems/two-variables.md)
