---
source: PRECALC
ref: "9.3 #9"
topics: [system-of-equations, nonlinear-system, substitution]
difficulty: intro
---

# Substitution

## Problem

Solve the system by substitution.

$$
\begin{cases}
y = -x \\
x^2 + y^2 = 9
\end{cases}
$$

## My attempt

**Label the equations.**

$$
\begin{aligned}
y &= -x && (1) \ \text{line} \\
x^2 + y^2 &= 9 && (2) \ \text{circle, radius 3}
\end{aligned}
$$

**Plan.** (1) already gives $y$: substitute it into (2).

**Step 1: substitute (1) into (2).**

$$
\begin{aligned}
x^2 + (-x)^2 &= 9 \\
x^2 + x^2 &= 9 \\
2x^2 &= 9 \\[6pt]
x^2 &= \frac{9}{2} \\[6pt]
x &= \pm\sqrt{\frac{9}{2}} = \pm\frac{3}{\sqrt{2}} \cdot \frac{\sqrt{2}}{\sqrt{2}} = \pm\frac{3\sqrt{2}}{2}
\end{aligned}
$$

**Step 2: back-substitute into (1).** The minus flips $\pm$ into $\mp$:

$$
y = -\left(\pm\frac{3\sqrt{2}}{2}\right) = \mp\frac{3\sqrt{2}}{2}
$$

So $x$ and $y$ have **opposite** signs.

**Check in both original equations.** Let $a = \frac{3\sqrt{2}}{2}$, so $a^2 = \frac{18}{4} = \frac{9}{2}$.
The pairs are $(a, -a)$ and $(-a, a)$; both have the same squares, so one check of (2)
covers both.

| Eq. | Substitution | Result |
|---|---|---|
| (1) | $y = -x$: $-a = -(a)$ and $a = -(-a)$ | $\checkmark$ |
| (2) | $a^2 + (-a)^2 = \frac{9}{2} + \frac{9}{2}$ | $9 \ \checkmark$ |

**Answer.** $\left(\frac{3\sqrt{2}}{2},\ -\frac{3\sqrt{2}}{2}\right)$ and
$\left(-\frac{3\sqrt{2}}{2},\ \frac{3\sqrt{2}}{2}\right)$.

## Mistake / lesson

## Related

- [Systems of nonlinear equations and inequalities](../../../notes/algebra/nonlinear-systems/two-variables.md)
