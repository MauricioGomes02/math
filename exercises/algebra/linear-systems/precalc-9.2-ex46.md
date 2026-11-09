---
source: PRECALC
ref: "9.2 #46"
topics: [system-of-equations, three-variables, elimination, fractions]
difficulty: hard
---

# Elimination with shifted variables

## Problem

Solve the system.

$$
\begin{cases}
x + y + z = 3 \\
\dfrac{x - 1}{2} + \dfrac{y - 3}{2} + \dfrac{z + 1}{2} = 0 \\
\dfrac{x - 2}{3} + \dfrac{y + 4}{3} + \dfrac{z - 3}{3} = \dfrac{2}{3}
\end{cases}
$$

## My attempt

**Label the equations.** (1) is already simple: $x + y + z = 3$.

**Step 1: clear the fractions in (2):** (2) × 2.

$$
\begin{aligned}
(x - 1) + (y - 3) + (z + 1) &= 0 \\
x + y + z - 3 &= 0 \\
x + y + z &= 3 && (2')
\end{aligned}
$$

**Step 2: clear the fractions in (3):** (3) × 3.

$$
\begin{aligned}
(x - 2) + (y + 4) + (z - 3) &= 2 \\
x + y + z - 1 &= 2 \\
x + y + z &= 3 && (3')
\end{aligned}
$$

**Observation.** (1), (2') and (3') are the same equation, so the three equations describe
the same plane: the system is **consistent and dependent** (infinitely many solutions).

**Step 3: solve for $z$** and leave $x$ and $y$ free:

$$
z = 3 - x - y
$$

**Check in all three original equations** with $x = 1$, $y = 1$, giving $(1, 1, 1)$:

| Eq. | Substitution | Result |
|---|---|---|
| (1) | $1 + 1 + 1$ | $3 \ \checkmark$ |
| (2) | $\dfrac{1 - 1}{2} + \dfrac{1 - 3}{2} + \dfrac{1 + 1}{2} = 0 - 1 + 1$ | $0 \ \checkmark$ |
| (3) | $\dfrac{1 - 2}{3} + \dfrac{1 + 4}{3} + \dfrac{1 - 3}{3} = \dfrac{-1 + 5 - 2}{3}$ | $\dfrac{2}{3} \ \checkmark$ |

**Answer.** Infinitely many solutions: $(x,\ y,\ 3 - x - y)$ for any real $x, y$.

## Mistake / lesson

## Related

- [Systems of linear equations in three variables](../../../notes/algebra/linear-systems/three-variables.md)
