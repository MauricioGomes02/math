---
source: PRECALC
ref: "9.2 #6"
topics: [system-of-equations, three-variables]
difficulty: intro
---

# Is (0, 1, −1) a solution?

## Problem

Determine whether $(0, 1, -1)$ is a solution of the system

$$
\begin{cases}
2x - 6y + 6z = -12 \\
x + 4y + 5z = -1 \\
-x + 2y + 3z = -1
\end{cases}
$$

## My attempt

**First equation** ($2x - 6y + 6z = -12$):

$$
2(0) - 6(1) + 6(-1) = 0 - 6 - 6 = -12 \ \checkmark
$$

**Second equation** ($x + 4y + 5z = -1$):

$$
(0) + 4(1) + 5(-1) = 0 + 4 - 5 = -1 \ \checkmark
$$

**Third equation** ($-x + 2y + 3z = -1$):

$$
-(0) + 2(1) + 3(-1) = 0 + 2 - 3 = -1 \ \checkmark
$$

**Answer.** $(0,\ 1,\ -1)$ satisfies all three equations, so it **is** a solution of the system.

## Mistake / lesson

- **Substitute from the problem statement, not from the previous line** (repeated from
  [9.1 #7](precalc-9.1-ex07.md)). I copied the first equation's $-6y$ pattern into the second and
  wrote $-4(1)$ instead of $+4(1)$. Writing the equation next to each check (as above) helps.
- **To say "is a solution", check every equation.** One failed equation is enough to say "no",
  but "yes" needs all three.

## Related

- [Systems of linear equations in three variables](../../../notes/algebra/linear-systems/three-variables.md)
