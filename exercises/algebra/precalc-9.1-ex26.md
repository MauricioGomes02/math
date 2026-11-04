---
source: PRECALC
ref: "9.1 #26"
topics: [system-of-equations, elimination]
difficulty: intermediate
---

# Addition method

## Problem

Solve by addition:

$$
\begin{cases}
7x + 6y = 2 \\
-28x - 24y = -8
\end{cases}
$$

## My attempt

**Divide the second equation by 4:**

$$
\begin{aligned}
\frac{-28x - 24y}{4} &= \frac{-8}{4} \\[6pt]
-7x - 6y &= -2
\end{aligned}
$$

**Add the equations:**

$$
\begin{aligned}
7x + 6y &= 2 \\
-7x - 6y &= -2 \\
\hline
0x + 0y &= 0 \\
0 &= 0
\end{aligned}
$$

**Conclusion.** Both variables cancel and the result is a true statement, so the system is
dependent: infinitely many solutions (both equations describe the same line).

**Express the solution set.** Solve the first equation for $y$:

$$
\begin{aligned}
7x + 6y &= 2 \\
6y &= 2 - 7x \\
y &= \frac{2 - 7x}{6}
\end{aligned}
$$

**Confirm with the second equation** (substitution gives an identity, as expected):

$$
\begin{aligned}
-28x - 24\left(\frac{2 - 7x}{6}\right) &= -8 \\
-28x - 4(2 - 7x) &= -8 \quad \left(\tfrac{-24}{6} = -4\right) \\
-28x - 8 + 28x &= -8 \\
-8 &= -8
\end{aligned}
$$

**Answer.** Every pair of the form

$$
\left(x,\ \frac{2 - 7x}{6}\right), \quad x \in \mathbb{R}
$$

**Check with one point** ($x = \tfrac{2}{7} \Rightarrow y = \tfrac{2 - 2}{6} = 0$):

- $7\left(\tfrac{2}{7}\right) + 6(0) = 2$ ✓
- $-28\left(\tfrac{2}{7}\right) - 24(0) = -8$ ✓

## Mistake / lesson

- **Dependent system ⇒ the answer is a set, not a point.** After getting $0 = 0$, I tried to find a
  single $x$. $\left(\tfrac{2}{7}, 0\right)$ is only *one* of the infinitely many solutions.
  Write the answer as $(x,\ y(x))$ for any real $x$.
- **Distribute a factor once.** In $-24\left(\frac{2 - 7x}{6}\right)$ I multiplied the numerator by
  $-24$ and still kept the $-24$ outside, applying it twice. Simplify $\frac{-24}{6} = -4$ first,
  then distribute.
- **Check in both original equations**, not just one.

## Related

- [Systems of linear equations](../../notes/algebra/systems-of-linear-equations.md)
