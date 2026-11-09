---
source: PRECALC
ref: "9.2 #51"
topics: [system-of-equations, three-variables, word-problem]
difficulty: intermediate
---

# Three even numbers

## Problem

Three even numbers sum up to 108. The smaller is half the larger and the middle number is
$\frac{3}{4}$ the larger. What are the three numbers?

## My attempt

**Model.** $x$ = smallest number, $y$ = middle number, $z$ = largest number.

$$
\begin{aligned}
x + y + z &= 108 && (1) \ \text{sum} \\
x &= \frac{z}{2} && (2) \ \text{smallest is half the largest} \\[6pt]
y &= \frac{3}{4}z && (3) \ \text{middle is } \tfrac{3}{4} \text{ of the largest}
\end{aligned}
$$

**Plan.** (2) and (3) already give $x$ and $y$ in terms of $z$, so substitute them into (1).

**Step 1: substitute (2) and (3) into (1).**

$$
\begin{aligned}
\frac{z}{2} + \frac{3z}{4} + z &= 108 \\[6pt]
\frac{2z + 3z + 4z}{4} &= 108 \\[6pt]
\frac{9z}{4} &= 108 \\[6pt]
9z &= 432 \\
z &= 48
\end{aligned}
$$

**Step 2: back-substitute** $z = 48$ into (2) and (3).

$$
\begin{aligned}
x &= \frac{48}{2} = 24 \\[6pt]
y &= \frac{3}{4}(48) = 36
\end{aligned}
$$

**Check every condition of the problem** with $(24, 36, 48)$:

| Condition | Substitution | Result |
|---|---|---|
| sum is 108 | $24 + 36 + 48$ | $108 \ \checkmark$ |
| smallest is half the largest | $\frac{48}{2}$ | $24 \ \checkmark$ |
| middle is $\frac{3}{4}$ of the largest | $\frac{3}{4}(48)$ | $36 \ \checkmark$ |
| all even | $24,\ 36,\ 48$ | even $\checkmark$ |

**Answer.** The three numbers are **24, 36 and 48**.

## Mistake / lesson

- **In a word problem, define the variables first** (what $x$, $y$, $z$ stand for), so each
  equation can be traced back to a sentence of the problem.
- **Answer the question that was asked**, in words, not only $x$, $y$, $z$.
- **Check every condition of the statement**, including ones not used in the equations
  (here: "even").

## Related

- [Systems of linear equations in three variables](../../../notes/algebra/linear-systems/three-variables.md)
