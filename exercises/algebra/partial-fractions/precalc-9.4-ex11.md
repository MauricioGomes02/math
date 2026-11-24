---
source: PRECALC
ref: "9.4 #11"
topics: [partial-fractions, linear-factors, factoring]
difficulty: intermediate
---

# Nonrepeated linear factors

## Problem

Find the decomposition of the partial fraction for the nonrepeating linear factors.

$$
\frac{32x - 11}{20x^2 - 13x + 2}
$$

## My attempt

**Plan.** Factor the denominator with the quadratic formula, write one fraction for each linear
factor, find the constants by equating coefficients, then simplify.

**Step 1: discriminant of the denominator** ($a = 20$, $b = -13$, $c = 2$).

$$
\Delta = (-13)^2 - 4 \cdot 20 \cdot 2 = 169 - 160 = 9 > 0 \quad \text{(two real roots)}
$$

**Step 2: roots.**

$$
\begin{aligned}
x &= \frac{-(-13) \pm \sqrt{9}}{2 \cdot 20} = \frac{13 \pm 3}{40} \\[6pt]
x_1 &= \frac{13 + 3}{40} = \frac{16}{40} = \frac{2}{5} \\[6pt]
x_2 &= \frac{13 - 3}{40} = \frac{10}{40} = \frac{1}{4}
\end{aligned}
$$

**Step 3: factored form** $a(x - x_1)(x - x_2)$, with the $20$ multiplied into the first factor.

$$
20x^2 - 13x + 2 = 20\left(x - \frac{2}{5}\right)\left(x - \frac{1}{4}\right)
= (20x - 8)\left(x - \frac{1}{4}\right)
$$

**Step 4: write the decomposition.**

$$
\frac{32x - 11}{(20x - 8)\left(x - \frac{1}{4}\right)} = \frac{A}{20x - 8} + \frac{B}{x - \frac{1}{4}} \qquad (1)
$$

**Step 5: multiply both sides of (1) by $(20x - 8)\left(x - \frac{1}{4}\right)$.**

$$
\begin{aligned}
32x - 11 &= A\left(x - \frac{1}{4}\right) + B(20x - 8) && (2) \\[6pt]
32x - 11 &= Ax - \frac{1}{4}A + 20Bx - 8B \\[6pt]
32x - 11 &= (A + 20B)\,x + \left(-\frac{1}{4}A - 8B\right)
\end{aligned}
$$

**Step 6: equate coefficients.**

$$
\begin{aligned}
x: \quad A + 20B &= 32 && (3) \\
\text{constant:} \quad -\frac{1}{4}A - 8B &= -11 && (4)
\end{aligned}
$$

**Step 7: (3) + (4) × 4** (the $A$ terms cancel)

$$
\begin{aligned}
A + 20B &= 32 \\
-A - 32B &= -44 \\
\hline
-12B &= -12 \\[6pt]
B &= 1
\end{aligned}
$$

**Step 8: substitute $B = 1$ into (3).**

$$
\begin{aligned}
A + 20(1) &= 32 \\
A &= 12
\end{aligned}
$$

**Check the system** with $A = 12$, $B = 1$:

| Eq. | Substitution | Result |
|---|---|---|
| (3) | $12 + 20(1)$ | $32$ $\checkmark$ |
| (4) | $-\frac{1}{4}(12) - 8(1) = -3 - 8$ | $-11$ $\checkmark$ |

**Step 9: put the constants into (1) and simplify.** Factor $20x - 8 = 4(5x - 2)$, and multiply
the second fraction by $\frac{4}{4}$ to clear the $\frac{1}{4}$:

$$
\begin{aligned}
\frac{12}{20x - 8} + \frac{1}{x - \frac{1}{4}}
&= \frac{12}{4(5x - 2)} + \frac{1}{x - \frac{1}{4}} \cdot \frac{4}{4} \\[6pt]
&= \frac{3}{5x - 2} + \frac{4}{4x - 1}
\end{aligned}
$$

The new denominators multiply back to the original one:
$(5x - 2)(4x - 1) = 20x^2 - 5x - 8x + 2 = 20x^2 - 13x + 2$ $\checkmark$.

**Check the decomposition:** recombine over $(5x - 2)(4x - 1)$. The numerator must be
$32x - 11$.

$$
\begin{aligned}
\frac{3}{5x - 2} + \frac{4}{4x - 1}
&= \frac{3(4x - 1) + 4(5x - 2)}{(5x - 2)(4x - 1)} \\[6pt]
&= \frac{12x - 3 + 20x - 8}{20x^2 - 13x + 2} \\[6pt]
&= \frac{32x - 11}{20x^2 - 13x + 2} \ \checkmark
\end{aligned}
$$

| Part | Original | Recombined | |
|---|---|---|---|
| Coefficient of $x$ | $32$ | $12 + 20 = 32$ | $\checkmark$ |
| Constant | $-11$ | $-3 - 8 = -11$ | $\checkmark$ |

**Answer.**

$$
\frac{32x - 11}{20x^2 - 13x + 2} = \frac{3}{5x - 2} + \frac{4}{4x - 1}
$$

## Mistake / lesson

- **Factor with integer coefficients:** when the leading coefficient is not $1$, split it
  between the factors ($20 = 5 \cdot 4$, so $5\left(x - \frac{2}{5}\right) = 5x - 2$ and
  $4\left(x - \frac{1}{4}\right) = 4x - 1$). The denominators then have no fractions, the system
  has whole numbers, and the answer comes out already simplified.

## Related

- [Partial fractions](../../../notes/algebra/partial-fractions/decomposition.md)
