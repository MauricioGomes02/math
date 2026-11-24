---
source: PRECALC
ref: "9.4 #21"
topics: [partial-fractions, repeated-linear-factors]
difficulty: intro
---

# Repeated linear factors

## Problem

Find the decomposition of the partial fraction for the repeating linear factors.

$$
\frac{x}{(x - 2)^2}
$$

## My attempt

**Plan.** The denominator is already factored. A repeated factor $(x - 2)^2$ needs one fraction
for each power ($1$ and $2$). Then find the constants by equating coefficients.

**Step 1: write the decomposition.**

$$
\frac{x}{(x - 2)^2} = \frac{A}{x - 2} + \frac{B}{(x - 2)^2} \qquad (1)
$$

**Step 2: multiply both sides of (1) by $(x - 2)^2$.**

$$
\begin{aligned}
(x - 2)^2 \cdot \frac{x}{(x - 2)^2} &= (x - 2)^2 \cdot \frac{A}{x - 2} + (x - 2)^2 \cdot \frac{B}{(x - 2)^2} \\[6pt]
x &= A(x - 2) + B && (2) \\[6pt]
x &= Ax - 2A + B \\[6pt]
x &= A\,x + (-2A + B)
\end{aligned}
$$

**Step 3: equate coefficients.** $B$ is a constant, so it does not go with the $x$ term.

$$
\begin{aligned}
x: \quad A &= 1 && (3) \\
\text{constant:} \quad -2A + B &= 0 && (4)
\end{aligned}
$$

**Step 4: substitute (3) into (4).**

$$
\begin{aligned}
-2(1) + B &= 0 \\
B &= 2
\end{aligned}
$$

Shortcut: with $x = 2$ in (2), the $A$ term vanishes: $2 = A \cdot 0 + B$, so $B = 2$ $\checkmark$.

**Check the system** with $A = 1$, $B = 2$:

| Eq. | Substitution | Result |
|---|---|---|
| (3) | $A = 1$ | $1$ $\checkmark$ |
| (4) | $-2(1) + 2$ | $0$ $\checkmark$ |

**Check the decomposition:** recombine over $(x - 2)^2$. The numerator must be $x$.

$$
\begin{aligned}
\frac{1}{x - 2} + \frac{2}{(x - 2)^2}
&= \frac{1 \cdot (x - 2) + 2}{(x - 2)^2} \\[6pt]
&= \frac{x - 2 + 2}{(x - 2)^2} \\[6pt]
&= \frac{x}{(x - 2)^2} \ \checkmark
\end{aligned}
$$

**Answer.**

$$
\frac{x}{(x - 2)^2} = \frac{1}{x - 2} + \frac{2}{(x - 2)^2}
$$

## Mistake / lesson

- **Equating coefficients:** in $x = Ax - 2A + B$, I first wrote $A + B = 1$ for the $x$ term.
  Only $A$ multiplies $x$; $B$ is a constant and belongs to the constant equation. Before
  writing the system, group the right side as $(\ldots)\,x + (\ldots)$.
- **Sign when substituting:** I wrote $-2A$ with $A = 1$ as $+2$. It is $-2(1) = -2$, so
  $B = 2$. Put the value in parentheses, $-2(1)$, to keep the sign.
- **Use the root shortcut as a check:** $x = 2$ in (2) gives $B$ in one line and catches both
  mistakes above.

## Related

- [Partial fractions](../../../notes/algebra/partial-fractions/decomposition.md)
