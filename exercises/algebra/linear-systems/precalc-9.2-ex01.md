---
source: PRECALC
ref: "9.2 #1"
topics: [system-of-equations, three-variables, proof]
difficulty: intro
---

# Can a system of three equations have exactly two solutions?

## Problem

Can a linear system of three equations have exactly two solutions? Explain why or why not.

## My attempt

**No.**

Each equation is a plane in space, and a solution is a point that lies on **all three** planes.

- If the three planes share at least one point, the system is **consistent**.
- If there is no point common to all three, the system is **inconsistent** (no solution).

The possible cases:

| Planes | Solutions |
|---|---|
| meet at a single point | exactly one |
| no point common to all three | none |
| meet along a line, or are the same plane | infinitely many |

**Why not exactly two.** Suppose the system has two different solutions $P$ and $Q$. Then each
plane contains both $P$ and $Q$. A plane that contains two points contains the **whole line**
through them, so every point of line $PQ$ lies on all three planes. That gives infinitely many
solutions, not two.

So a linear system of three equations has 0, 1 or infinitely many solutions, never exactly two.

## Mistake / lesson

- **Justify the key step.** My first version didn't explain why two solutions are impossible
  (same lesson as [9.1 #1](precalc-9.1-ex01.md)). The reason: a plane that contains two points
  contains the whole line through them.
- **With three planes, "meet" means all three at once.** Two planes can cross each other while
  the third misses that line, so pairwise meetings are not enough for a solution.

## Related

- [Systems of linear equations in three variables](../../../notes/algebra/linear-systems/three-variables.md)
- [PRECALC 9.1 #1](precalc-9.1-ex01.md) (same question with two variables)
