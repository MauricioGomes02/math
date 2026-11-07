---
source: PRECALC
ref: "9.2 #17"
topics: [system-of-equations, three-variables, elimination]
difficulty: intermediate
---

# Elimination with a missing variable

## Problem

Solve the system.

$$
\begin{cases}
2x - y + 3z = 17 \\
-5x + 4y - 2z = -46 \\
2y + 5z = -7
\end{cases}
$$

## My attempt

**Label the equations.**

$$
\begin{aligned}
2x - y + 3z &= 17 && (1) \\
-5x + 4y - 2z &= -46 && (2) \\
2y + 5z &= -7 && (3)
\end{aligned}
$$

**Plan.** Eliminate $y$ twice, with two different pairs: (1) with (2) and (1) with (3).

**Step 1: (1) × 4 + (2)** (makes $-4y$ and $+4y$)

$$
\begin{aligned}
8x - 4y + 12z &= 68 \\
-5x + 4y - 2z &= -46 \\
\hline
3x + 10z &= 22 && (4)
\end{aligned}
$$

**Step 2: (1) × 2 + (3)** (makes $-2y$ and $+2y$)

$$
\begin{aligned}
4x - 2y + 6z &= 34 \\
2y + 5z &= -7 \\
\hline
4x + 11z &= 27 && (5)
\end{aligned}
$$

**Step 3: solve the $2 \times 2$ system (4), (5).** Eliminate $x$: (4) × 4 and (5) × (−3).

$$
\begin{aligned}
12x + 40z &= 88 \\
-12x - 33z &= -81 \\
\hline
7z &= 7 \\
z &= 1
\end{aligned}
$$

**Step 4: back-substitute.** $z = 1$ in (4):

$$
\begin{aligned}
3x + 10(1) &= 22 \\
3x &= 12 \\
x &= 4
\end{aligned}
$$

$x = 4$, $z = 1$ in (1):

$$
\begin{aligned}
2(4) - y + 3(1) &= 17 \\
11 - y &= 17 \\
-y &= 6 \\
y &= -6
\end{aligned}
$$

**Check in all three original equations** with $(4, -6, 1)$:

| Eq. | Substitution | Result |
|---|---|---|
| (1) | $2(4) - (-6) + 3(1) = 8 + 6 + 3$ | $17 \ \checkmark$ |
| (2) | $-5(4) + 4(-6) - 2(1) = -20 - 24 - 2$ | $-46 \ \checkmark$ |
| (3) | $2(-6) + 5(1) = -12 + 5$ | $-7 \ \checkmark$ |

**Answer.** $(x, y, z) = (4,\ -6,\ 1)$.

## Mistake / lesson

- **Use the missing variable.** Equation (3) has no $x$. Eliminating $x$ once from (1) and (2)
  gives a second equation in $y, z$, and together with (3) that is already a $2 \times 2$
  system: one elimination instead of two. Before starting, look for an equation that is
  missing a variable.
- **The plan must match the steps.** I copied the plan from [ex11](precalc-9.2-ex11.md)
  ("(1) + (2)"), but Step 1 here is (1) × 4 + (2).
- **Clean up before finishing.** The first version had leftover lines (equations pasted outside
  `$$` and a stray $\frac{8}{3}$ in the check table) and a missing `\\` that broke a line.

## Related

- [Systems of linear equations in three variables](../../../notes/algebra/linear-systems/three-variables.md)
