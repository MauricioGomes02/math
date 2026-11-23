---
source: PRECALC
ref: "9.4 #6"
topics: [partial-fractions, linear-factors]
difficulty: intro
---

# Nonrepeated linear factors

## Problem

Find the decomposition of the partial fraction for the nonrepeating linear factors.

$$
\frac{5x + 16}{x^2 + 10x + 24}
$$

## My attempt

**Plan.** Factor the denominator, write one fraction for each linear factor, then find the
constants $A$ and $B$.

**Step 1: factor the denominator.** Sum and product suggests $(x + 4)(x + 6)$
($4 + 6 = 10$, $4 \cdot 6 = 24$). To confirm it, find the roots with the quadratic formula
($a = 1$, $b = 10$, $c = 24$):

$$
\begin{aligned}
\Delta &= b^2 - 4ac = 10^2 - 4(1)(24) = 100 - 96 = 4 > 0 \quad \text{(two real roots)} \\[6pt]
x &= \frac{-10 \pm \sqrt{4}}{2 \cdot 1} = \frac{-10 \pm 2}{2} \\[6pt]
x_1 &= \frac{-10 + 2}{2} = \frac{-8}{2} = -4 \\[6pt]
x_2 &= \frac{-10 - 2}{2} = \frac{-12}{2} = -6
\end{aligned}
$$

With the factored form $a(x - x_1)(x - x_2)$:

$$
x^2 + 10x + 24 = 1\,[x - (-4)]\,[x - (-6)] = (x + 4)(x + 6)
$$

**Step 2: write the decomposition.** Two nonrepeated linear factors, so one constant over each:

$$
\frac{5x + 16}{(x + 4)(x + 6)} = \frac{A}{x + 4} + \frac{B}{x + 6} \qquad (1)
$$

**Step 3: multiply both sides of (1) by $(x + 4)(x + 6)$** to clear the denominators.

$$
\begin{aligned}
(x + 4)(x + 6) \cdot \frac{5x + 16}{(x + 4)(x + 6)}
  &= (x + 4)(x + 6) \cdot \frac{A}{x + 4} + (x + 4)(x + 6) \cdot \frac{B}{x + 6} \\[6pt]
5x + 16 &= A(x + 6) + B(x + 4) && (2)
\end{aligned}
$$

**Step 4: expand (2) and group by powers of $x$.**

$$
\begin{aligned}
5x + 16 &= Ax + 6A + Bx + 4B \\[6pt]
5x + 16 &= (A + B)\,x + (6A + 4B)
\end{aligned}
$$

**Step 5: equate coefficients.** Both sides must be the same polynomial, so the coefficients of
$x$ match and the constants match:

$$
\begin{aligned}
x: \quad A + B &= 5 && (3) \\
\text{constant:} \quad 6A + 4B &= 16 \ \Rightarrow \ 3A + 2B = 8 && (4)
\end{aligned}
$$

**Step 6: (3) × (−2) + (4)** (the $B$ terms cancel)

$$
\begin{aligned}
-2A - 2B &= -10 \\
3A + 2B &= 8 \\
\hline
A &= -2
\end{aligned}
$$

**Step 7: substitute $A = -2$ into (3).**

$$
\begin{aligned}
-2 + B &= 5 \\
B &= 7
\end{aligned}
$$

**Check the system** with $A = -2$, $B = 7$:

| Eq. | Substitution | Result |
|---|---|---|
| (3) | $-2 + 7$ | $5$ $\checkmark$ |
| (4) | $3(-2) + 2(7) = -6 + 14$ | $8$ $\checkmark$ |

**Step 8: put $A = -2$ and $B = 7$ back into (1).**

$$
\frac{5x + 16}{(x + 4)(x + 6)} = -\frac{2}{x + 4} + \frac{7}{x + 6}
$$

**Check the decomposition:** add the pieces back over the common denominator
$(x + 4)(x + 6)$. The numerator must be $5x + 16$.

$$
\begin{aligned}
-\frac{2}{x + 4} + \frac{7}{x + 6}
&= \frac{-2(x + 6) + 7(x + 4)}{(x + 4)(x + 6)} \\[6pt]
&= \frac{-2x - 12 + 7x + 28}{(x + 4)(x + 6)} \\[6pt]
&= \frac{5x + 16}{(x + 4)(x + 6)} \ \checkmark
\end{aligned}
$$

| Part | Original | Recombined | |
|---|---|---|---|
| Coefficient of $x$ | $5$ | $-2 + 7 = 5$ | $\checkmark$ |
| Constant | $16$ | $-12 + 28 = 16$ | $\checkmark$ |

**Answer.**

$$
\frac{5x + 16}{x^2 + 10x + 24} = -\frac{2}{x + 4} + \frac{7}{x + 6}
$$

## Mistake / lesson

- **Constants swapped:** I first wrote $\frac{7}{x + 4} - \frac{2}{x + 6}$. In (1), $A$ sits over
  $x + 4$ and $B$ over $x + 6$, so it is $\frac{-2}{x + 4} + \frac{7}{x + 6}$. Recombining
  catches it: $7(x + 6) - 2(x + 4) = 5x + 34 \ne 5x + 16$.
- **Factored form of a quadratic:** I wrote the structure as $a(x_1 - x_2)^2$. It is
  $a(x - x_1)(x - x_2)$: one factor per root, each with $x$ in it.

## Related

- [Partial fractions](../../../notes/algebra/partial-fractions/decomposition.md)
