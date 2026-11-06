---
source: PRECALC
ref: "9.1 #19"
topics: [system-of-equations, substitution, fractions]
difficulty: hard
---

# Substitution with fractions

## Problem

Solve by substitution:

$$
\begin{cases}
\frac{1}{2}x + \frac{1}{3}y = 16 \\[4pt]
\frac{1}{6}x + \frac{1}{4}y = 9
\end{cases}
$$

## My attempt

**Clear the fractions** (multiply each equation by a common multiple of its denominators):

$$
\begin{aligned}
6\left(\frac{1}{2}x + \frac{1}{3}y\right) &= 6(16) \\[6pt]
24\left(\frac{1}{6}x + \frac{1}{4}y\right) &= 24(9)
\end{aligned}
$$

$$
\begin{cases}
3x + 2y = 96 \\
4x + 6y = 216
\end{cases}
$$

**Solve the first equation for $y$:**

$$
\begin{aligned}
2y &= 96 - 3x \\[6pt]
y &= \frac{96 - 3x}{2}
\end{aligned}
$$

**Substitute into the second equation:**

$$
\begin{aligned}
4x + 6\left(\frac{96 - 3x}{2}\right) &= 216 \\[6pt]
4x + 3(96 - 3x) &= 216 \quad \left(\tfrac{6}{2} = 3\right) \\[6pt]
4x + 288 - 9x &= 216 \\[6pt]
-5x &= -72 \\[6pt]
x &= \frac{72}{5}
\end{aligned}
$$

**Substitute $x$ back to find $y$:**

$$
\begin{aligned}
3\left(\frac{72}{5}\right) + 2y &= 96 \\[6pt]
\frac{216}{5} + 2y &= 96 \\[6pt]
2y &= \frac{480 - 216}{5} = \frac{264}{5} \\[6pt]
y &= \frac{264}{5} \cdot \frac{1}{2} = \frac{132}{5}
\end{aligned}
$$

**Check in both original equations** (with fractions):

- $\frac{1}{2}\cdot\frac{72}{5} + \frac{1}{3}\cdot\frac{132}{5} = \frac{36}{5} + \frac{44}{5} = \frac{80}{5} = 16$ ✓
- $\frac{1}{6}\cdot\frac{72}{5} + \frac{1}{4}\cdot\frac{132}{5} = \frac{12}{5} + \frac{33}{5} = \frac{45}{5} = 9$ ✓

**Answer.** $\left(\frac{72}{5},\ \frac{132}{5}\right) = (14.4,\ 26.4)$

## Mistake / lesson

- **Use the least common multiple.** For the second equation I multiplied by 24, but the LCM of
  6 and 4 is **12**. Any common multiple clears the fractions, but the LCM keeps numbers small:
  $2x + 3y = 108$ instead of $4x + 6y = 216$.
- **Simplify before distributing.** $6 \cdot \frac{96 - 3x}{2} = 3(96 - 3x)$, since $\frac{6}{2} = 3$
  (same lesson as [ex26](precalc-9.1-ex26.md)).
- **Check in the original equations, not the transformed ones.** Checking in the fraction-free
  system doesn't catch a mistake made while clearing the fractions.

## Related

- [Systems of linear equations](../../notes/algebra/systems-of-linear-equations.md)
