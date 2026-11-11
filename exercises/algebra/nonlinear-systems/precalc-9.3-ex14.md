---
source: PRECALC
ref: "9.3 #14"
topics: [system-of-equations, nonlinear-system, elimination]
difficulty: intermediate
---

# Elimination

## Problem

Solve the system by elimination.

$$
\begin{cases}
y^2 - x^2 = 9 \\
3x^2 + 2y^2 = 8
\end{cases}
$$

## My attempt

**Label the equations.**

$$
\begin{aligned}
y^2 - x^2 &= 9 && (1) \ \text{hyperbola} \\
3x^2 + 2y^2 &= 8 && (2) \ \text{ellipse}
\end{aligned}
$$

**Plan.** Neither equation is linear, but both have only $x^2$ and $y^2$: treat them as the
variables and eliminate $y^2$.

**Step 1: (1) × (−2) + (2)** (makes $-2y^2$ and $+2y^2$)

$$
\begin{aligned}
2x^2 - 2y^2 &= -18 \\
3x^2 + 2y^2 &= 8 \\
\hline
5x^2 &= -10 \\
x^2 &= -2
\end{aligned}
$$

No real number squared is negative, so there is no real $x$.

**Graph check.** From (1), $y^2 = 9 + x^2 \ge 9$, so the hyperbola only exists where
$|y| \ge 3$. From (2), $2y^2 \le 8$, so the ellipse only exists where $|y| \le 2$. The curves
live in separate bands and never meet.

**Answer.** No real solution.

## Mistake / lesson

## Related

- [Systems of nonlinear equations and inequalities](../../../notes/algebra/nonlinear-systems/two-variables.md)
