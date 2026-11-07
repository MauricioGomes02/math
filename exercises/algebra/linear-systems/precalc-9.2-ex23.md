---
source: PRECALC
ref: "9.2 #23"
topics: [system-of-equations, three-variables, elimination]
difficulty: intermediate
---

# Elimination

## Problem

Solve the system.

$$
\begin{cases}
x + y + z = 14 \\
2y + 3z = -14 \\
-16y - 24z = -112
\end{cases}
$$

## My attempt

**Label the equations.**

$$
\begin{aligned}
x + y + z &= 14 && (1) \\
2y + 3z &= -14 && (2) \\
-16y - 24z &= -112 && (3)
\end{aligned}
$$

**Observation.** The left side of (3) is $-8$ times the left side of (2), but the constant is
not: $-8 \times (-14) = 112 \neq -112$. Planes (2) and (3) are parallel.

**Plan.** (2) and (3) already have only $y$ and $z$, so combine them directly.

**Step 1: (2) × 8 + (3)**

$$
\begin{aligned}
16y + 24z &= -112 \\
-16y - 24z &= -112 \\
\hline
0 &= -224
\end{aligned}
$$

Both variables cancel and $0 = -224$ is false, so (2) and (3) have no common point. No
value of $x$ in (1) can change that.

**Answer.** The system is **inconsistent**: no solution.

## Mistake / lesson

## Related

- [Systems of linear equations in three variables](../../../notes/algebra/linear-systems/three-variables.md)
