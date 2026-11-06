---
source: PRECALC
ref: "9.1 #21"
topics: [system-of-equations, elimination]
difficulty: intermediate
---

# Addition method

## Problem

Solve by addition:

$$
\begin{cases}
-2x + 5y = -42 \\
7x + 2y = 30
\end{cases}
$$

## My attempt

**Multiply the first equation by $\frac{7}{2}$:**

$$
\begin{aligned}
\frac{7(-2x + 5y)}{2} &= \frac{7(-42)}{2} \\[6pt]
-7x + \frac{35y}{2} &= -147 \\[6pt]
\end{aligned}
$$

**Add the equations:**

$$
\begin{aligned}
-7x + \frac{35y}{2} &= -147 \\[6pt]
7x + 2y &= 30 \\
\hline
\frac{35y + 4y}{2} &= -117
\end{aligned}
$$

**Solve for $y$:**

$$
\begin{aligned}
\frac{39y}{2} &= -117 \\[6pt]
39y &= -234 \\[6pt]
y &= -\frac{234}{39} = -6
\end{aligned}
$$

**Substitute $y$ into the first equation to find $x$:**

$$
\begin{aligned}
-2x + 5(-6) &= -42 \\
-2x - 30 &= -42 \\
-2x &= -12 \\
x &= \frac{-12}{-2} = 6
\end{aligned}
$$

**Check in both original equations.**

- $-2(6) + 5(-6) = -12 - 30 = -42$ ✓
- $7(6) + 2(-6) = 42 - 12 = 30$ ✓

**Answer.** $(6,\ -6)$

## Mistake / lesson

- **Prefer integer multipliers.** Scaling by $\tfrac{7}{2}$ works but introduces fractions
  ($\tfrac{35y}{2} + 2y$). When the coefficients aren't multiples of each other, multiply **both**
  equations by integers instead: first by 7, second by 2 gives $-14x$ and $14x$, and everything
  stays whole numbers.

## Related

- [Systems of linear equations](../../notes/algebra/systems-of-linear-equations.md)
