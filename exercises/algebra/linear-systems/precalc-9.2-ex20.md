---
source: PRECALC
ref: "9.2 #20"
topics: [system-of-equations, three-variables, elimination]
difficulty: intermediate
---

# Elimination

## Problem

Solve the system.

$$
\begin{cases}
4x + 6y - 2z = 8 \\
6x + 9y - 3z = 12 \\
-2x - 3y + z = -4
\end{cases}
$$

## My attempt

**Label the equations.**

$$
\begin{aligned}
4x + 6y - 2z &= 8 && (1) \\
6x + 9y - 3z &= 12 && (2) \\
-2x - 3y + z &= -4 && (3)
\end{aligned}
$$

**Observation.** The coefficients are proportional: $(1) = -2 \times (3)$ and
$(2) = -3 \times (3)$. All three equations describe the same plane.

**Plan.** Eliminate $x$ with two different pairs, (1) with (2) and (1) with (3), and see
what is left.

**Step 1: (1) ÷ 2 + (2) ÷ (−3)**

$$
\begin{aligned}
2x + 3y - z &= 4 \\
-2x - 3y + z &= -4 \\
\hline
0 &= 0
\end{aligned}
$$

**Step 2: (1) ÷ 2 + (3)**

$$
\begin{aligned}
2x + 3y - z &= 4 \\
-2x - 3y + z &= -4 \\
\hline
0 &= 0
\end{aligned}
$$

Every variable cancels and $0 = 0$ is always true, so the system is **consistent and
dependent**: infinitely many solutions.

**Solve (3) for $z$** (coefficient $1$):

$$
\begin{aligned}
-2x - 3y + z &= -4 \\
z &= 2x + 3y - 4
\end{aligned}
$$

$x$ and $y$ are free (any real numbers).

**Check in all three original equations** with $x = 0$, $y = 0$, giving $(0, 0, -4)$:

| Eq. | Substitution | Result |
|---|---|---|
| (1) | $4(0) + 6(0) - 2(-4) = 0 + 0 + 8$ | $8 \ \checkmark$ |
| (2) | $6(0) + 9(0) - 3(-4) = 0 + 0 + 12$ | $12 \ \checkmark$ |
| (3) | $-2(0) - 3(0) + (-4)$ | $-4 \ \checkmark$ |

**Answer.** Infinitely many solutions: $(x,\ y,\ 2x + 3y - 4)$ for any real $x, y$.

## Mistake / lesson

- **Proportional equations mean the same plane, not "no system".** My first version said
  elimination was impossible and that there was no solution. Elimination works and gives
  $0 = 0$; three copies of the same plane share every point of it, so there are infinitely
  many solutions.
- **Dividing by a negative flips every term.** In Step 1 I wrote $(2) \div (-3)$ as
  $-2x - 3y - z = 4$; the $z$ term and the constant must flip too: $+z = -4$.
- **Check in the equations you didn't use.** I first checked $(0, 0, -4)$ only in (3), the
  equation $z$ came from, which always passes (same lesson as [9.1 #26](precalc-9.1-ex26.md)).

## Related

- [Systems of linear equations in three variables](../../../notes/algebra/linear-systems/three-variables.md)
- [PRECALC 9.1 #26](precalc-9.1-ex26.md) (dependent system in two variables)
