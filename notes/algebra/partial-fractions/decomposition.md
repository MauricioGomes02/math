---
topics: [partial-fractions, rational-expressions, linear-factors, quadratic-factors, system-of-equations]
sources: [PRECALC 9.4]
---

# Partial fractions

## Definition

**Partial fraction decomposition** rewrites a rational expression $\frac{P(x)}{Q(x)}$ as a sum
of simpler fractions, one for each factor of the denominator $Q(x)$. For example:

$$
\frac{3x}{(x + 2)(x - 1)} = \frac{A}{x + 2} + \frac{B}{x - 1}
$$

The goal is to find the constants ($A$, $B$, …).

## Intuition

It is **adding fractions in reverse**. Adding $\frac{2}{x + 2} + \frac{1}{x - 1}$ gives one
fraction over the common denominator $(x + 2)(x - 1)$. Decomposition starts from that single
fraction and recovers the pieces. (It is used later in calculus, where the small pieces are
much easier to work with than the big fraction.)

## Before you start

1. **The fraction must be proper:** degree of $P(x)$ < degree of $Q(x)$. If not, first do
   polynomial long division and decompose only the remainder part.
2. **Factor the denominator completely** into linear factors $(ax + b)$ and irreducible
   quadratic factors $(ax^2 + bx + c$ with $b^2 - 4ac < 0)$. Useful patterns:
   - $a^2 - b^2 = (a - b)(a + b)$
   - $a^3 - b^3 = (a - b)(a^2 + ab + b^2)$
   - $a^3 + b^3 = (a + b)(a^2 - ab + b^2)$

## The four cases

Each factor of $Q(x)$ contributes its own terms:

| Factor in $Q(x)$ | Terms in the decomposition |
|---|---|
| nonrepeated linear $(ax + b)$ | $\dfrac{A}{ax + b}$ |
| repeated linear $(ax + b)^n$ | $\dfrac{A_1}{ax + b} + \dfrac{A_2}{(ax + b)^2} + \dots + \dfrac{A_n}{(ax + b)^n}$ |
| nonrepeated irreducible quadratic $(ax^2 + bx + c)$ | $\dfrac{Ax + B}{ax^2 + bx + c}$ |
| repeated irreducible quadratic $(ax^2 + bx + c)^n$ | $\dfrac{A_1x + B_1}{ax^2 + bx + c} + \dots + \dfrac{A_nx + B_n}{(ax^2 + bx + c)^n}$ |

Rule of thumb: the numerator over a quadratic is **linear** ($Ax + B$); over a linear factor it
is a **constant**. A repeated factor needs **one term for each power**, from $1$ up to $n$.

## Finding the constants

1. Write the decomposition with unknown constants.
2. **Multiply both sides by $Q(x)$** to clear all denominators.
3. Find the constants with one (or both) of these methods:
   - **Plug in convenient $x$ values:** choose the roots of the linear factors, so all terms but
     one become $0$. Fast for linear factors.
   - **Equate coefficients:** expand, group by powers of $x$, and set the coefficients of
     $x^2$, $x$ and the constant equal on both sides. This gives a **linear system** (as in
     9.1 and 9.2). Needed for quadratic factors.

**Example (PRECALC 9.4, Example 1):**

$$
\begin{aligned}
\frac{3x}{(x + 2)(x - 1)} &= \frac{A}{x + 2} + \frac{B}{x - 1} \\[6pt]
3x &= A(x - 1) + B(x + 2)
\end{aligned}
$$

- $x = 1$: the $A$ term vanishes, $3 = 3B$, so $B = 1$.
- $x = -2$: the $B$ term vanishes, $-6 = -3A$, so $A = 2$.

$$
\frac{3x}{(x + 2)(x - 1)} = \frac{2}{x + 2} + \frac{1}{x - 1}
$$

## Checking

Add the pieces back over the common denominator. The numerator must match $P(x)$ exactly. In the
example: $2(x - 1) + 1(x + 2) = 3x$ $\checkmark$.

## Common mistakes

- Decomposing an improper fraction without dividing first.
- Stopping before the denominator is fully factored (e.g. leaving $x^3 - 1$ as is).
- Writing only $\frac{A}{(x - 2)^2}$ for a repeated factor and forgetting $\frac{A_1}{x - 2}$.
- Putting a constant $A$ over a quadratic factor instead of $Ax + B$.
- Forgetting a constant factor such as the $2$ in $2x^2 + 12x + 18 = 2(x + 3)^2$.
- Sign errors when plugging in negative roots.

## Exercises

| Exercise | Topic | Difficulty |
|---|---|---|
| [ex01](../../../exercises/algebra/partial-fractions/precalc-9.4-ex01.md) | Concept (verbal) | intro |
| [ex06](../../../exercises/algebra/partial-fractions/precalc-9.4-ex06.md) | Nonrepeated linear factors | intro |
| [ex21](../../../exercises/algebra/partial-fractions/precalc-9.4-ex21.md) | Repeated linear factors | intro |
| [ex11](../../../exercises/algebra/partial-fractions/precalc-9.4-ex11.md) | Nonrepeated linear factors | intermediate |
| [ex26](../../../exercises/algebra/partial-fractions/precalc-9.4-ex26.md) | Repeated linear factors | intermediate |
| [ex27](../../../exercises/algebra/partial-fractions/precalc-9.4-ex27.md) | Repeated linear factors | intermediate |
| [ex31](../../../exercises/algebra/partial-fractions/precalc-9.4-ex31.md) | Irreducible quadratic factor | intermediate |
| [ex37](../../../exercises/algebra/partial-fractions/precalc-9.4-ex37.md) | Irreducible quadratic factor | intermediate |
| [ex45](../../../exercises/algebra/partial-fractions/precalc-9.4-ex45.md) | Repeated quadratic factor | intermediate |
| [ex41](../../../exercises/algebra/partial-fractions/precalc-9.4-ex41.md) | Irreducible quadratic factor | hard |
| [ex51](../../../exercises/algebra/partial-fractions/precalc-9.4-ex51.md) | Repeated quadratic factor | hard |
| [ex55](../../../exercises/algebra/partial-fractions/precalc-9.4-ex55.md) | Partial fraction expansion | hard |

## See also

- [Systems of linear equations in three variables](../linear-systems/three-variables.md)
- [Systems of linear equations in two variables](../linear-systems/two-variables.md)
