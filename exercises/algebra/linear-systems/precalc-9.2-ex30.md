---
source: PRECALC
ref: "9.2 #30"
topics: [system-of-equations, three-variables, elimination, fractions]
difficulty: hard
---

# Elimination with fractions

## Problem

Solve the system.

$$
\begin{cases}
\frac{1}{2}x - \frac{1}{5}y + \frac{2}{5}z = -\frac{13}{10} \\
\frac{1}{4}x - \frac{2}{5}y - \frac{1}{5}z = -\frac{7}{20} \\
-\frac{1}{2}x - \frac{3}{4}y - \frac{1}{2}z = -\frac{5}{4}
\end{cases}
$$

## My attempt

**Clear fractions and label the equations:** (1) × 10, (2) × 20, (3) × 4.

$$
\begin{aligned}
5x - 2y + 4z &= -13 && (1') \\
5x - 8y - 4z &= -7 && (2') \\
-2x - 3y - 2z &= -5 && (3')
\end{aligned}
$$

**Plan.** Eliminate $z$ twice, with two different pairs: (1') with (2') and (1') with (3').

**Step 1: (1') + (2')** (the $z$ coefficients are already opposite)

$$
\begin{aligned}
5x - 2y + 4z &= -13 \\
5x - 8y - 4z &= -7 \\
\hline
10x - 10y &= -20 \\
x - y &= -2 && (4)
\end{aligned}
$$

**Step 2: (1') + (3') × 2** (makes $4z$ and $-4z$)

$$
\begin{aligned}
5x - 2y + 4z &= -13 \\
-4x - 6y - 4z &= -10 \\
\hline
x - 8y &= -23 && (5)
\end{aligned}
$$

**Step 3: solve the $2 \times 2$ system (4), (5).** Eliminate $x$: (4) + (5) × (−1).

$$
\begin{aligned}
x - y &= -2 \\
-x + 8y &= 23 \\
\hline
7y &= 21 \\
y &= 3
\end{aligned}
$$

**Step 4: back-substitute.** $y = 3$ in (4):

$$
\begin{aligned}
x - 3 &= -2 \\
x &= 1
\end{aligned}
$$

$x = 1$, $y = 3$ in (1'):

$$
\begin{aligned}
5(1) - 2(3) + 4z &= -13 \\
-1 + 4z &= -13 \\
4z &= -12 \\
z &= -3
\end{aligned}
$$

**Check in all three original equations** (with fractions) with $(1, 3, -3)$:

| Eq. | Substitution | Result |
|---|---|---|
| (1) | $\frac{1}{2}(1) - \frac{1}{5}(3) + \frac{2}{5}(-3) = \frac{5}{10} - \frac{6}{10} - \frac{12}{10}$ | $-\frac{13}{10} \ \checkmark$ |
| (2) | $\frac{1}{4}(1) - \frac{2}{5}(3) - \frac{1}{5}(-3) = \frac{5}{20} - \frac{24}{20} + \frac{12}{20}$ | $-\frac{7}{20} \ \checkmark$ |
| (3) | $-\frac{1}{2}(1) - \frac{3}{4}(3) - \frac{1}{2}(-3) = -\frac{2}{4} - \frac{9}{4} + \frac{6}{4}$ | $-\frac{5}{4} \ \checkmark$ |

**Answer.** $(x, y, z) = (1,\ 3,\ -3)$.

## Mistake / lesson

- **Check in the original equations, not the cleared ones.** Checking only the equations
  without fractions can't catch a mistake made while clearing them.

## Related

- [Systems of linear equations in three variables](../../../notes/algebra/linear-systems/three-variables.md)
