---
source: PRECALC
ref: "9.3 #19"
topics: [system-of-equations, nonlinear-system, elimination, completing-the-square]
difficulty: intermediate
---

# Any method

## Problem

Solve the system using any method.

$$
\begin{cases}
x^2 + y^2 = 1 \\
y = -x^2
\end{cases}
$$

## My attempt

**Label the equations.**

$$
\begin{aligned}
x^2 + y^2 &= 1 && (1) \ \text{circle, radius 1} \\
y &= -x^2 && (2) \ \text{parabola, vertex } (0, 0) \text{, opens down}
\end{aligned}
$$

**What to expect.** The vertex $(0, 0)$ is inside the circle and the parabola opens down
and leaves it, so the curves must cross.

**Step 1: write (2) in the same form as (1).**

$$
-x^2 - y = 0 \qquad (2')
$$

**Step 2: (1) + (2')** (the $x^2$ terms cancel)

$$
\begin{aligned}
x^2 + y^2 &= 1 \\
-x^2 - y &= 0 \\
\hline
y^2 - y &= 1 \\
y^2 - y - 1 &= 0
\end{aligned}
$$

**Step 3: complete the square.** Half the linear coefficient, squared:
$\left(-\frac{1}{2}\right)^2 = \frac{1}{4}$. Add $1 + \frac{1}{4}$ to both sides.

$$
\begin{aligned}
y^2 - y + \frac{1}{4} &= \frac{5}{4} \\[6pt]
\left(y - \frac{1}{2}\right)^2 &= \frac{5}{4} \\[6pt]
y - \frac{1}{2} &= \pm\frac{\sqrt{5}}{2} \\[6pt]
y &= \frac{1 \pm \sqrt{5}}{2}
\end{aligned}
$$

**Step 4: find $x^2$ for each $y$** (substitute into (1)).

$y = \frac{1 + \sqrt{5}}{2}$:

$$
\begin{aligned}
x^2 + \frac{5 + 2\sqrt{5} + 1}{4} &= 1 \\[6pt]
x^2 + \frac{3 + \sqrt{5}}{2} &= 1 \\[6pt]
x^2 &= \frac{-1 - \sqrt{5}}{2} < 0
\end{aligned}
$$

A square can't be negative, so this $y$ gives **no point**.

$y = \frac{1 - \sqrt{5}}{2}$:

$$
\begin{aligned}
x^2 + \frac{5 - 2\sqrt{5} + 1}{4} &= 1 \\[6pt]
x^2 + \frac{3 - \sqrt{5}}{2} &= 1 \\[6pt]
x^2 &= \frac{-1 + \sqrt{5}}{2} > 0 \\[6pt]
x &= \pm\sqrt{\frac{-1 + \sqrt{5}}{2}} = \pm\frac{\sqrt{-2 + 2\sqrt{5}}}{2}
\end{aligned}
$$

This $y$ gives **two points**, one for each sign of $x$.

**Check in both original equations.** Both pairs have $x^2 = \frac{-1 + \sqrt{5}}{2}$ and
$y = \frac{1 - \sqrt{5}}{2}$, so one check covers both.

| Eq. | Substitution | Result |
|---|---|---|
| (1) | $\frac{-1 + \sqrt{5}}{2} + \frac{6 - 2\sqrt{5}}{4} = \frac{-1 + \sqrt{5}}{2} + \frac{3 - \sqrt{5}}{2} = \frac{2}{2}$ | $1 \ \checkmark$ |
| (2) | $-x^2 = -\frac{-1 + \sqrt{5}}{2} = \frac{1 - \sqrt{5}}{2}$ | $y \ \checkmark$ |

**Answer.** $\left(\frac{\sqrt{-2 + 2\sqrt{5}}}{2},\ \frac{1 - \sqrt{5}}{2}\right)$ and
$\left(-\frac{\sqrt{-2 + 2\sqrt{5}}}{2},\ \frac{1 - \sqrt{5}}{2}\right)$.

## Mistake / lesson

- **Completing the square uses the same half you squared.** I added $\frac{1}{4} =
  \left(-\frac{1}{2}\right)^2$ but wrote $(y - 1)^2$; it must be $\left(y - \frac{1}{2}\right)^2$.
- **The $\pm$ goes on the root only.** First I dropped it (and lost the $y$ that gives the
  solutions), then put it in front of everything: $\pm\frac{\sqrt{5} + 1}{2}$. The
  $\frac{1}{2}$ didn't come from a root: $y = \frac{1 \pm \sqrt{5}}{2}$.
- **$(a + b)^2 \neq a^2 + b^2$.** The middle term $2ab$ is missing. Substituting into (2),
  $x^2 = -y$, avoids squaring altogether.
- **From $x^2 = k$ to $x$, take the root:** $x = \pm\sqrt{k}$, not $x = \pm k$.
- **Sketch first.** The picture showed the curves must cross, so "no real solution" was a sign
  of an error.

## Related

- [Systems of nonlinear equations and inequalities](../../../notes/algebra/nonlinear-systems/two-variables.md)
