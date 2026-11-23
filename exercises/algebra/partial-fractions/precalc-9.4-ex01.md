---
source: PRECALC
ref: "9.4 #1"
topics: [partial-fractions, concept]
difficulty: intro
---

# Can every fraction be decomposed?

## Problem

*(Verbal question, paraphrased.)* Can any quotient of polynomials be decomposed into at
least two partial fractions? If so, explain why. If not, give an example of a fraction that
cannot be decomposed.

## My attempt

**Answer: no.** Each partial fraction has one factor of the denominator as its own
denominator. To split a fraction into **at least two** pieces, the denominator must factor into
**at least two** factors. Some denominators cannot be factored.

**Example.**

$$
\frac{1}{x^2 + 1}
$$

**Why $x^2 + 1$ does not factor.** With $a = 1$, $b = 0$, $c = 1$:

$$
b^2 - 4ac = 0^2 - 4(1)(1) = -4 < 0
$$

The discriminant is negative, so $x^2 + 1$ has no real roots and no real linear factors: it is
an **irreducible** quadratic. The fraction has a single factor in the denominator and is already
in its simplest form.

**Another case:** a denominator with a single linear factor, such as $\frac{5}{x - 3}$, cannot
be split either.

**What about the degree of the numerator?** The book's method requires a **proper** fraction:
degree of $P(x)$ < degree of $Q(x)$. When that fails, polynomial long division turns the
fraction into one that satisfies it:

$$
\frac{P(x)}{Q(x)} = \text{polynomial} + \frac{R(x)}{Q(x)}, \qquad \deg R < \deg Q
$$

and $\frac{R(x)}{Q(x)}$ is then decomposed. For example,
$\frac{x^2}{x^2 - 1} = 1 + \frac{1}{x^2 - 1}$. So the degree is a condition of the method, not
a reason the decomposition is impossible.

## Mistake / lesson

- **Difference of squares:** I factored $x^2 + 1$ as $(x + 1)(x - 1)$, but
  $(x + 1)(x - 1) = x^2 - x + x - 1 = x^2 - 1$. The last product is $1 \cdot (-1) = -1$. Check a
  factoring by multiplying it back, or with the discriminant.
- **Degree of the numerator is not a blocker:** an improper fraction can still be decomposed
  after long division; it is an extra step, not a reason for "no".
- **Give a fraction as the example:** the question asks for a fraction, so the example is
  $\frac{1}{x^2 + 1}$, not the polynomial $x^2 + 1$.

## Related

- [Partial fractions](../../../notes/algebra/partial-fractions/decomposition.md)
