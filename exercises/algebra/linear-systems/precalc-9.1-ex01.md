---
source: PRECALC
ref: "9.1 #1"
topics: [system-of-equations, proof]
difficulty: intro
---

# Can a linear system have exactly two solutions?

## Problem

Can a linear system of two equations in two variables have exactly two solutions? Explain why or why not.

## My attempt

**No.**

Each equation is a line in the plane, and a solution is a point where the lines meet.

- If the lines meet at some point, the system is **consistent**.
- If they never meet, the system is **inconsistent** (no solution).

What happens depends on the slope $m$ and the $y$-intercept $b$ of each line ($y = mx + b$):

| Slopes | Intercepts | Lines | Solutions |
|---|---|---|---|
| different | — | cross once | exactly one |
| same | different | parallel | none |
| same | same | same line | infinitely many |

**Why not exactly two.** Suppose the lines share two different points. Through two different
points there is **only one line**, so both equations describe that same line. Then they share
every point on it, which means infinitely many solutions, not two.

So a linear system has 0, 1 or infinitely many solutions, never exactly two.

## Mistake / lesson

- **Justify the key step, don't just state it.** My first version said "for two solutions the
  lines must overlap" without saying why. The reason is a geometric fact: two different points
  determine exactly one line.
- **In a yes/no question, start with the answer**, then explain.

## Related

- [Systems of linear equations](../../../notes/algebra/linear-systems/two-variables.md)
