---
source: PRECALC
ref: "9.2 #37"
topics: [system-of-equations, three-variables, elimination, decimals]
difficulty: hard
---

# Elimination with decimals

## Problem

Solve the system.

$$
\begin{cases}
0.1x - 0.2y + 0.3z = 2 \\
0.5x - 0.1y + 0.4z = 8 \\
0.7x - 0.2y + 0.3z = 8
\end{cases}
$$

## My attempt

**Clear decimals and label the equations:** (1) × 10, (2) × 10, (3) × 10.

$$
\begin{aligned}
x - 2y + 3z &= 20 && (1') \\
5x - y + 4z &= 80 && (2') \\
7x - 2y + 3z &= 80 && (3')
\end{aligned}
$$

**Plan.** Eliminate $y$ twice, with two different pairs: (1') with (2') and (1') with (3').

**Step 1: (1') + (2') × (−2)** (makes $-2y$ and $+2y$)

$$
\begin{aligned}
x - 2y + 3z &= 20 \\
-10x + 2y - 8z &= -160 \\
\hline
-9x - 5z &= -140 && (4)
\end{aligned}
$$

**Step 2: (1') + (3') × (−1)** (makes $-2y$ and $+2y$)

$$
\begin{aligned}
x - 2y + 3z &= 20 \\
-7x + 2y - 3z &= -80 \\
\hline
-6x &= -60 \\
3x &= 30 && (5)
\end{aligned}
$$

**Step 3: solve the $2 \times 2$ system (4), (5).** Eliminate $x$: (4) + (5) × 3.

$$
\begin{aligned}
-9x - 5z &= -140 \\
9x &= 90 \\
\hline
-5z &= -50 \\
z &= 10
\end{aligned}
$$

**Step 4: back-substitute.** $z = 10$ in (4):

$$
\begin{aligned}
-9x - 5(10) &= -140 \\
-9x &= -90 \\
x &= 10
\end{aligned}
$$

$x = 10$, $z = 10$ in (1'):

$$
\begin{aligned}
10 - 2y + 3(10) &= 20 \\
40 - 2y &= 20 \\
-2y &= -20 \\
y &= 10
\end{aligned}
$$

**Check in all three original equations** (with decimals) with $(10, 10, 10)$:

| Eq. | Substitution | Result |
|---|---|---|
| (1) | $0.1(10) - 0.2(10) + 0.3(10) = 1 - 2 + 3$ | $2 \ \checkmark$ |
| (2) | $0.5(10) - 0.1(10) + 0.4(10) = 5 - 1 + 4$ | $8 \ \checkmark$ |
| (3) | $0.7(10) - 0.2(10) + 0.3(10) = 7 - 2 + 3$ | $8 \ \checkmark$ |

**Answer.** $(x, y, z) = (10,\ 10,\ 10)$.

## Mistake / lesson

- **Look at what each step already gives before following the plan.** (1') and (3') share
  $-2y + 3z$, so Step 2 cancelled $y$ **and** $z$ and gave $x = 10$ directly. Putting $x = 10$
  into (4) gives $z$ right away; Step 3 and solving for $x$ again in Step 4 were not needed.

## Related

- [Systems of linear equations in three variables](../../../notes/algebra/linear-systems/three-variables.md)
