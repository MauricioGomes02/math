---
source: PRECALC
ref: "9.2 #11"
topics: [system-of-equations, three-variables, elimination]
difficulty: intermediate
---

# Elimination

## Problem

Solve the system by elimination.

$$
\begin{cases}
3x - 4y + 2z = -15 \\
2x + 4y + z = 16 \\
2x + 3y + 5z = 20
\end{cases}
$$

## My attempt

**Label the equations.**

$$
\begin{aligned}
3x - 4y + 2z &= -15 && (1) \\
2x + 4y + z &= 16 && (2) \\
2x + 3y + 5z &= 20 && (3)
\end{aligned}
$$

**Plan.** Eliminate $y$ twice, with two different pairs: (1) + (2) and (1) with (3).

**Step 1: (1) + (2)** (the $y$ coefficients are already opposite)

$$
\begin{aligned}
3x - 4y + 2z &= -15 \\
2x + 4y + z &= 16 \\
\hline
5x + 3z &= 1 && (4)
\end{aligned}
$$

**Step 2: (1) × 3 + (3) × 4** (makes $-12y$ and $+12y$)

$$
\begin{aligned}
9x - 12y + 6z &= -45 \\
8x + 12y + 20z &= 80 \\
\hline
17x + 26z &= 35 && (5)
\end{aligned}
$$

**Step 3: solve the $2 \times 2$ system (4), (5).** Eliminate $x$: (4) × 17 and (5) × (−5).

$$
\begin{aligned}
85x + 51z &= 17 \\
-85x - 130z &= -175 \\
\hline
-79z &= -158 \\
z &= 2
\end{aligned}
$$

**Step 4: back-substitute.** $z = 2$ in (4):

$$
\begin{aligned}
5x + 3(2) &= 1 \\
5x &= -5 \\
x &= -1
\end{aligned}
$$

$x = -1$, $z = 2$ in (2):

$$
\begin{aligned}
2(-1) + 4y + 2 &= 16 \\
4y &= 16 \\
y &= 4
\end{aligned}
$$

**Check in all three original equations** with $(-1, 4, 2)$:

| Eq. | Substitution | Result |
|---|---|---|
| (1) | $3(-1) - 4(4) + 2(2) = -3 - 16 + 4$ | $-15 \ \checkmark$ |
| (2) | $2(-1) + 4(4) + 2 = -2 + 16 + 2$ | $16 \ \checkmark$ |
| (3) | $2(-1) + 3(4) + 5(2) = -2 + 12 + 10$ | $20 \ \checkmark$ |

**Answer.** $(x, y, z) = (-1,\ 4,\ 2)$.

## Mistake / lesson

- **Add every column when combining equations.** In Step 2, I wrote $9x + 8x = x$
  (subtracted instead of adding). One slip in one column made every later number wrong.
- **A failed check means "find the error", not "no solution".** "No solution" only comes from a
  false statement like $0 = 5$ during elimination. A failed check means an arithmetic mistake
  (same lesson as [9.1 #27](precalc-9.1-ex27.md)).
- **Ugly numbers are a warning sign.** A denominator like $127$ in a textbook exercise usually
  means a slip. Re-check the last combination before going on.
- **Re-add each combination column by column** ($x$, then $y$, then $z$, then the constant)
  before moving on. It takes seconds and catches most slips.
- **Label equations and write the operation**, e.g. "(1) × 3 + (3) × 4", so each step can be
  re-checked without redoing everything.

## Related

- [Systems of linear equations in three variables](../../../notes/algebra/linear-systems/three-variables.md)
