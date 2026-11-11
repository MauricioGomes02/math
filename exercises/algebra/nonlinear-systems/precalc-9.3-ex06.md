---
source: PRECALC
ref: "9.3 #6"
topics: [system-of-equations, nonlinear-system, substitution, completing-the-square]
difficulty: intermediate
---

# Substitution

## Problem

Solve the system by substitution.

$$
\begin{cases}
x + y = 4 \\
x^2 + y^2 = 9
\end{cases}
$$

## My attempt

**Label the equations.**

$$
\begin{aligned}
x + y &= 4 && (1) \ \text{line} \\
x^2 + y^2 &= 9 && (2) \ \text{circle, radius 3}
\end{aligned}
$$

**Plan.** (1) is linear: solve it for $x$ and substitute into (2).

**Step 1: solve (1) for $x$.**

$$
x = 4 - y \qquad (3)
$$

**Step 2: substitute (3) into (2).**

$$
\begin{aligned}
(4 - y)^2 + y^2 &= 9 \\
16 - 8y + y^2 + y^2 &= 9 \\
2y^2 - 8y + 7 &= 0 \\[6pt]
y^2 - 4y + \frac{7}{2} &= 0
\end{aligned}
$$

**Step 3: complete the square.** Half the linear coefficient, squared:
$\left(\frac{4}{2}\right)^2 = 4$. The constant is $\frac{7}{2}$, so add $\frac{1}{2}$ to both
sides to reach $4$.

$$
\begin{aligned}
y^2 - 4y + 4 &= \frac{1}{2} \\[6pt]
(y - 2)^2 &= \frac{1}{2} \\[6pt]
y - 2 &= \pm\sqrt{\frac{1}{2}} = \pm\frac{\sqrt{2}}{2} \\[6pt]
y &= 2 \pm \frac{\sqrt{2}}{2}
\end{aligned}
$$

**Step 4: back-substitute into (3).** The minus in front flips $\pm$ into $\mp$:

$$
\begin{aligned}
x &= 4 - \left(2 \pm \frac{\sqrt{2}}{2}\right) \\[6pt]
x &= 2 \mp \frac{\sqrt{2}}{2}
\end{aligned}
$$

So $x$ and $y$ take **opposite** signs:

| $y$ | $x = 4 - y$ | Pair |
|---|---|---|
| $2 + \frac{\sqrt{2}}{2}$ | $2 - \frac{\sqrt{2}}{2}$ | $\left(2 - \frac{\sqrt{2}}{2},\ 2 + \frac{\sqrt{2}}{2}\right)$ |
| $2 - \frac{\sqrt{2}}{2}$ | $2 + \frac{\sqrt{2}}{2}$ | $\left(2 + \frac{\sqrt{2}}{2},\ 2 - \frac{\sqrt{2}}{2}\right)$ |

**Check in both original equations.** Let $a = \frac{\sqrt{2}}{2}$, so $a^2 = \frac{1}{2}$.
Both pairs are $(2 + a,\ 2 - a)$ in some order, so one check covers both:

| Eq. | Substitution | Result |
|---|---|---|
| (1) | $(2 + a) + (2 - a)$ | $4 \ \checkmark$ |
| (2) | $(2 + a)^2 + (2 - a)^2 = (4 + 4a + a^2) + (4 - 4a + a^2) = 8 + 2a^2 = 8 + 1$ | $9 \ \checkmark$ |

**Answer.** $\left(2 - \frac{\sqrt{2}}{2},\ 2 + \frac{\sqrt{2}}{2}\right)$ and
$\left(2 + \frac{\sqrt{2}}{2},\ 2 - \frac{\sqrt{2}}{2}\right)$.

## Mistake / lesson

- **A minus in front of $\pm$ flips it to $\mp$.** I wrote $4 - (2 \pm a) = 2 \pm a$, which
  pairs the signs wrongly; I had to recompute $y$ from each $x$ to fix the pairing.
- **Simplify roots:** $\sqrt{\frac{1}{2}} = \frac{\sqrt{2}}{2}$.
- **Check with a shortcut:** naming $a = \frac{\sqrt{2}}{2}$ makes the cross terms cancel at a
  glance ($+4a$ and $-4a$).

## Related

- [Systems of nonlinear equations and inequalities](../../../notes/algebra/nonlinear-systems/two-variables.md)
