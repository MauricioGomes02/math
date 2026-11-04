---
topics: [break-even, cost, revenue, profit, system-of-equations]
sources: [PRECALC 9.1]
---

# Break-even analysis

## Definition

For $x$ units produced and sold:

- **Cost** $C(x) = \text{(cost per unit)}\cdot x + \text{(fixed cost)}$
- **Revenue** $R(x) = \text{(price)}\cdot x$
- **Profit** $P(x) = R(x) - C(x)$

The **break-even point** is where $C(x) = R(x)$, i.e. $P(x) = 0$. It is the solution
of the system $\{\,y = C(x),\ y = R(x)\,\}$, written as the pair
$(\text{quantity},\ \text{money})$.

## Intuition

Fixed costs are a hole you start in. Each unit sold fills it by
$\text{price} - \text{cost per unit}$ (the **margin per unit**). Break-even is when the hole is full:

$$
x^* = \frac{\text{fixed cost}}{\text{price} - \text{cost per unit}}
$$

- Margin per unit $> 0$: profit after $x^*$.
- Margin per unit $\le 0$: no positive break-even; every sale loses money (or doesn't help).

## Worked example (PRECALC 9.1, Example 10)

$C(x) = 0.85x + 35{,}000$, $R(x) = 1.55x$.

$1.55x = 0.85x + 35{,}000 \Rightarrow 0.7x = 35{,}000 \Rightarrow x = 50{,}000$, and $R(50{,}000) = 77{,}500$.

Break-even: $(50{,}000,\ 77{,}500)$. Profit function: $P(x) = 0.7x - 35{,}000$.

## Common mistakes

- Reporting only $x$; the break-even point is the pair (units, money).
- Answering with a fractional unit count when the question asks "after how many units": round **up**.

## Exercises

- [precalc-9.1-ex56](../../exercises/algebra/precalc-9.1-ex56.md)
- [precalc-9.1-ex60](../../exercises/algebra/precalc-9.1-ex60.md)

## See also

- [Systems of linear equations](../algebra/systems-of-linear-equations.md)
