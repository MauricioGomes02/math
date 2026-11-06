---
source: PRECALC
ref: "9.1 #27"
topics: [system-of-equations, elimination, fractions]
difficulty: hard
---

# Addition method with fractions

## Problem

Solve by addition:

$$
\begin{cases}
\frac{5}{6}x + \frac{1}{4}y = 0 \\[4pt]
\frac{1}{8}x - \frac{1}{2}y = -\frac{43}{120}
\end{cases}
$$

## My attempt

**Scale the second equation by $\tfrac{1}{2}$** so the $y$ terms become opposites:

$$
\begin{aligned}
\frac{5}{6}x + \frac{1}{4}y &= 0 \\[6pt]
\frac{1}{16}x - \frac{1}{4}y &= -\frac{43}{240}
\end{aligned}
$$

**Add the equations** ($y$ cancels). Common denominator of 6 and 16 is 48:

$$
\frac{5}{6} + \frac{1}{16} = \frac{40}{48} + \frac{3}{48} = \frac{43}{48}
$$

$$
\begin{aligned}
\frac{43}{48}x &= -\frac{43}{240} \\[6pt]
x &= -\frac{43}{240} \cdot \frac{48}{43} = -\frac{48}{240} = -\frac{1}{5}
\end{aligned}
$$

**Substitute $x$ into the first original equation** to find $y$:

$$
\begin{aligned}
\frac{5}{6}\left(-\frac{1}{5}\right) + \frac{1}{4}y &= 0 \\[6pt]
-\frac{1}{6} + \frac{1}{4}y &= 0 \\[6pt]
\frac{1}{4}y &= \frac{1}{6} \\[6pt]
y &= \frac{1}{6} \cdot 4 = \frac{2}{3}
\end{aligned}
$$

**Check in both original equations.**

- $\frac{5}{6}\left(-\frac{1}{5}\right) + \frac{1}{4}\cdot\frac{2}{3} = -\frac{1}{6} + \frac{1}{6} = 0$ ✓
- $\frac{1}{8}\left(-\frac{1}{5}\right) - \frac{1}{2}\cdot\frac{2}{3} = -\frac{1}{40} - \frac{1}{3} = -\frac{3}{120} - \frac{40}{120} = -\frac{43}{120}$ ✓

**Answer.** $\left(-\frac{1}{5},\ \frac{2}{3}\right)$

## Mistake / lesson

- **Adding fractions:** first attempt computed $\frac{5}{6} + \frac{1}{16}$ as $\frac{46}{256}$.
  Rule: rewrite both over a common denominator (LCD of 6 and 16 is 48), then add numerators:
  $\frac{40}{48} + \frac{3}{48} = \frac{43}{48}$.
- **Simplifying:** $\frac{11008}{11040}$ was simplified to $\frac{345}{344}$ (fraction flipped).
  A number less than 1 cannot simplify to one greater than 1.
- **After finding $x$, stop solving for $x$.** Substitute it into an original equation to get $y$;
  don't use the value as a new coefficient.
- **Dividing by a fraction = multiplying by its reciprocal:** from $\frac{1}{4}y = k$, $y = 4k$, not $\frac{1}{4}k$.
- **A failed check means go back.** The first check gave $\ne 0$; that was the signal to look for the error.
- **Tip:** clear fractions first (multiply eq. 1 by 12 and eq. 2 by 120) to get an integer system and avoid
  most of these arithmetic slips.

## Related

- [Systems of linear equations](../../../notes/algebra/linear-systems/two-variables.md)
