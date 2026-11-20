---
source: PRECALC
ref: "9.3 #52"
topics: [system-of-equations, nonlinear-system]
difficulty: hard
---

# Any method

## Problem

Solve the system using any method.

$$
\begin{cases}
x^2 + 4xy - 2y^2 - 6 = 0 \\
x = y + 2
\end{cases}
$$

## My attempt

**Label the equations.**

$$
\begin{aligned}
x^2 + 4xy - 2y^2 - 6 &= 0 && (1) \\
x &= y + 2 && (2)
\end{aligned}
$$

**Plan.** (2) already gives $x$: substitute it into (1), solve the quadratic in $y$ by
completing the square, then get each $x$ from (2).

**Step 1: substitute (2) into (1).**

$$
\begin{aligned}
(y + 2)^2 + 4(y + 2)y - 2y^2 - 6 &= 0 \\[6pt]
(y^2 + 4y + 4) + (4y^2 + 8y) - 2y^2 - 6 &= 0 \\[6pt]
(y^2 + 4y^2 - 2y^2) + (4y + 8y) + (4 - 6) &= 0 \\[6pt]
3y^2 + 12y - 2 &= 0 && (3)
\end{aligned}
$$

**Step 2: (3) ÷ 3 and complete the square.** To turn $-\frac{2}{3}$ into
$\left(\frac{4}{2}\right)^2 = 4$, add $4 + \frac{2}{3}$ to both sides:

$$
\begin{aligned}
y^2 + 4y - \frac{2}{3} &= 0 \\[6pt]
y^2 + 4y - \frac{2}{3} + \left(4 + \frac{2}{3}\right) &= 0 + \left(4 + \frac{2}{3}\right) \\[6pt]
y^2 + 4y + 4 &= \frac{12 + 2}{3} \\[6pt]
(y + 2)^2 &= \frac{14}{3} \\[6pt]
y + 2 &= \pm\sqrt{\frac{14}{3}}
  = \pm\frac{\sqrt{14}}{\sqrt{3}} \cdot \frac{\sqrt{3}}{\sqrt{3}}
  = \pm\frac{\sqrt{42}}{3} \\[6pt]
y &= \pm\frac{\sqrt{42}}{3} - 2
\end{aligned}
$$

**Step 3: find each $x$ with (2).**

$$
\begin{aligned}
y = \frac{\sqrt{42}}{3} - 2: \quad x &= \left(\frac{\sqrt{42}}{3} - 2\right) + 2 = \frac{\sqrt{42}}{3} \\[10pt]
y = -\frac{\sqrt{42}}{3} - 2: \quad x &= \left(-\frac{\sqrt{42}}{3} - 2\right) + 2 = -\frac{\sqrt{42}}{3}
\end{aligned}
$$

Shortcut: by (2), $y + 2 = x$, so the line $(y + 2)^2 = \frac{14}{3}$ in Step 2 already says
$x^2 = \frac{14}{3}$.

**Check.** Write both solutions at once as $x = t$, $y = t - 2$ with $t = \pm\frac{\sqrt{42}}{3}$,
so $t^2 = \frac{14}{3}$. Simplify in terms of $t^2$ and only plug in the value at the end:

$$
\begin{aligned}
x^2 + 4xy - 2y^2 - 6
&= t^2 + 4t(t - 2) - 2(t - 2)^2 - 6 \\[6pt]
&= t^2 + 4t^2 - 8t - 2(t^2 - 4t + 4) - 6 \\[6pt]
&= t^2 + 4t^2 - 8t - 2t^2 + 8t - 8 - 6 \\[6pt]
&= 3t^2 - 14 \\[6pt]
&= 3 \cdot \frac{14}{3} - 14 = 0
\end{aligned}
$$

The $-8t$ and $+8t$ cancel, so the sign of $t$ does not matter: the check works for both
solutions.

| Eq. | Substitution | Result |
|---|---|---|
| (1) | $3t^2 - 14 = 3 \cdot \frac{14}{3} - 14$ | $0$ $\checkmark$ |
| (2) | $y + 2 = (t - 2) + 2$ | $t = x$ $\checkmark$ |

**Answer.**

$$
\left(\frac{\sqrt{42}}{3},\ \frac{\sqrt{42}}{3} - 2\right), \quad
\left(-\frac{\sqrt{42}}{3},\ -\frac{\sqrt{42}}{3} - 2\right)
$$

## Mistake / lesson

## Related

- [Systems of nonlinear equations and inequalities](../../../notes/algebra/nonlinear-systems/two-variables.md)
