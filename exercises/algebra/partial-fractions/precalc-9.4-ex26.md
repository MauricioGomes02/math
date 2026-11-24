---
source: PRECALC
ref: "9.4 #26"
topics: [partial-fractions, repeated-linear-factors, factoring]
difficulty: intermediate
---

# Repeated linear factors

## Problem

Find the decomposition of the partial fraction for the repeating linear factors.

$$
\frac{5x + 14}{2x^2 + 12x + 18}
$$

## My attempt

**Plan.** Factor the denominator with the discriminant, write the decomposition for the repeated
factor, find the constants by equating coefficients, then simplify.

**Step 1: discriminant of the denominator** ($a = 2$, $b = 12$, $c = 18$).

$$
\Delta = 12^2 - 4 \cdot 2 \cdot 18 = 144 - 144 = 0 \quad \text{(one double root)}
$$

**Step 2: the double root.**

$$
x = \frac{-12 \pm \sqrt{0}}{2 \cdot 2} = \frac{-12}{4} = -3
$$

**Step 3: factored form** $a(x - x_1)(x - x_2)$ with $x_1 = x_2 = -3$, the $2$ multiplied into
the first factor.

$$
2x^2 + 12x + 18 = 2\,[x - (-3)]\,[x - (-3)] = (2x + 6)(x + 3) = 2(x + 3)^2
$$

**Step 4: write the decomposition.** One fraction for each power of the repeated factor:

$$
\frac{5x + 14}{(2x + 6)(x + 3)} = \frac{A}{2x + 6} + \frac{B}{(x + 3)^2} \qquad (1)
$$

**Step 5: multiply both sides of (1) by $(2x + 6)(x + 3)$.** In the $B$ term,
$\frac{(2x + 6)(x + 3)}{(x + 3)^2} = \frac{2(x + 3)(x + 3)}{(x + 3)^2} = 2$.

$$
\begin{aligned}
5x + 14 &= A(x + 3) + 2B && (2) \\[6pt]
5x + 14 &= Ax + 3A + 2B \\[6pt]
5x + 14 &= A\,x + (3A + 2B)
\end{aligned}
$$

**Step 6: equate coefficients.**

$$
\begin{aligned}
x: \quad A &= 5 && (3) \\
\text{constant:} \quad 3A + 2B &= 14 && (4)
\end{aligned}
$$

**Step 7: substitute (3) into (4).**

$$
\begin{aligned}
3(5) + 2B &= 14 \\
2B &= 14 - 15 = -1 \\
B &= -\frac{1}{2}
\end{aligned}
$$

Shortcut: with $x = -3$ in (2), the $A$ term vanishes: $5(-3) + 14 = 2B$, so $-1 = 2B$ and
$B = -\frac{1}{2}$ $\checkmark$.

**Check the system** with $A = 5$, $B = -\frac{1}{2}$:

| Eq. | Substitution | Result |
|---|---|---|
| (3) | $A = 5$ | $5$ $\checkmark$ |
| (4) | $3(5) + 2\left(-\frac{1}{2}\right) = 15 - 1$ | $14$ $\checkmark$ |

**Step 8: put the constants into (1) and simplify.** Factor the $2$ out of $2x + 6$, and clear
the fraction inside the second fraction (dividing by $2$ is multiplying by $\frac{1}{2}$, so the
$2$ goes to the denominator):

$$
\begin{aligned}
\frac{5}{2x + 6} + \frac{-\frac{1}{2}}{(x + 3)^2}
&= \frac{5}{2(x + 3)} - \frac{1}{2} \cdot \frac{1}{(x + 3)^2} \\[6pt]
&= \frac{5}{2(x + 3)} - \frac{1}{2(x + 3)^2}
\end{aligned}
$$

**Check the decomposition:** recombine over $2(x + 3)^2$. The numerator must be $5x + 14$.

$$
\begin{aligned}
\frac{5}{2(x + 3)} - \frac{1}{2(x + 3)^2}
&= \frac{5(x + 3) - 1}{2(x + 3)^2} \\[6pt]
&= \frac{5x + 15 - 1}{2(x^2 + 6x + 9)} \\[6pt]
&= \frac{5x + 14}{2x^2 + 12x + 18} \ \checkmark
\end{aligned}
$$

**Answer.**

$$
\frac{5x + 14}{2x^2 + 12x + 18} = \frac{5}{2(x + 3)} - \frac{1}{2(x + 3)^2}
$$

## Mistake / lesson

- **No fraction inside a fraction:** $\frac{-\frac{1}{2}}{(x + 3)^2}$ is correct but not
  simplified. Dividing by $2$ moves the $2$ to the denominator: $-\frac{1}{2(x + 3)^2}$.

## Related

- [Partial fractions](../../../notes/algebra/partial-fractions/decomposition.md)
