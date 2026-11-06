---
source: PRECALC
ref: "9.1 #56"
topics: [system-of-equations, break-even]
difficulty: intermediate
---

# Break-even point

## Problem

A business making stuffed animals has cost $C = 12x + 30$ and revenue $R = 20x$,
where $x$ is the number of units. Find the break-even point.

## My attempt

**Model.**

$$
\begin{aligned}
C(x) &= 12x + 30 \\
R(x) &= 20x \\
R(x) &= C(x) \quad \text{(break-even, i.e. } R(x) - C(x) = 0\text{)}
\end{aligned}
$$

**System.**

$$
\begin{cases}
y = 12x + 30 \\
y = 20x
\end{cases}
$$

**Eliminate $y$** (add the first equation to $-1$ times the second):

$$
\begin{aligned}
-8x + 30 &= 0 \\
8x &= 30 \\
x &= \frac{30}{8} = 3.75
\end{aligned}
$$

**Check.** $C(3.75) = 12(3.75) + 30 = 45 + 30 = 75$ and $R(3.75) = 20(3.75) = 75$ ✓

**Answer.** Break-even point: $(3.75,\ 75)$.

## Mistake / lesson

## Related

- [Break-even analysis](../../../notes/economics/break-even.md)
- [Systems of linear equations](../../../notes/algebra/linear-systems/two-variables.md)
