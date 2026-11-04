---
source: PRECALC
ref: "9.1 #60"
topics: [system-of-equations, break-even, pricing]
difficulty: hard
---

# Break-even price

## Problem

A guitar factory has cost $C(x) = 75x + 50{,}000$. The company needs to break even after
150 units are sold. At what price should each guitar be sold? Round up to the nearest
dollar and write the revenue function.

## My attempt

**Model.** The unknown is the price $p$; the quantity is given ($x = 150$).

$$
\begin{aligned}
C(x) &= 75x + 50000 \\
R(x) &= px \\
R(x) - C(x) &= 0 \quad \text{(break-even)}
\end{aligned}
$$

**Evaluate at $x = 150$.**

$$
\begin{aligned}
y &= 75(150) + 50000 = 11250 + 50000 = 61250 \\
y &= 150p
\end{aligned}
$$

**Eliminate $y$** (add the first equation to $-1$ times the second):

$$
\begin{aligned}
61250 - 150p &= 0 \\
p &= \frac{61250}{150} = 408.33\ldots
\end{aligned}
$$

**Round up** (the problem requires it):

$$
p = \lceil 408.33\ldots \rceil = 409
$$

**Answer.** Price: $409 per guitar. Revenue function:

$$
R(x) = 409x
$$

**Check.** $R(150) = 409 \cdot 150 = 61350 \ge 61250 = C(150)$ ✓

## Mistake / lesson

- **First attempt:** wrote $R(x) = 150x$, treating 150 as the *price*. It was the *quantity*.
  Before writing equations, list what is **known** and what is **unknown**:
  here $x = 150$ is given and the price $p$ is the unknown.
- **Revenue is always price × quantity:** $R(x) = p \cdot x$.
- **Rounding direction matters.** $408.33$ would normally round to $408$, but at $p = 408$
  revenue is $61200 < 61250$, so the company would not break even. When the question asks for a
  minimum price to cover a cost, round **up** ($\lceil\cdot\rceil$).
- **Always check the result in the original problem.**

## Related

- [Break-even analysis](../../notes/economics/break-even.md)
- [Systems of linear equations](../../notes/algebra/systems-of-linear-equations.md)
