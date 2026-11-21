---
source: PRECALC
ref: "9.3 #55"
topics: [system-of-equations, nonlinear-system, word-problem]
difficulty: intermediate
---

# Two numbers

## Problem

Two numbers add up to 300. One number is twice the square of the other number. What are the
numbers?

## My attempt

**Define the variables.** Let $y$ be one number and $x$ the other, with $x$ being twice the
square of $y$.

**Label the equations.**

$$
\begin{aligned}
x + y &= 300 && (1) \\
x &= 2y^2 && (2)
\end{aligned}
$$

**Plan.** Isolate $x$ in (1), substitute into (2), solve the quadratic in $y$ by completing
the square, then get each $x$ from (1).

**Step 1: isolate $x$ in (1).**

$$
x = 300 - y \qquad (3)
$$

**Step 2: substitute (3) into (2).**

$$
\begin{aligned}
300 - y &= 2y^2 \\[6pt]
2y^2 + y - 300 &= 0 && (4)
\end{aligned}
$$

**Step 3: (4) ÷ 2 and complete the square.** Half of $\frac{1}{2}$ is $\frac{1}{4}$, and
$\left(\frac{1}{4}\right)^2 = \frac{1}{16}$, so add $\frac{1}{16} + 150$ to both sides:

$$
\begin{aligned}
y^2 + \frac{1}{2}y - 150 &= 0 \\[6pt]
y^2 + \frac{1}{2}y - 150 + \left(\frac{1}{16} + 150\right) &= 0 + \left(\frac{1}{16} + 150\right) \\[6pt]
y^2 + \frac{1}{2}y + \frac{1}{16} &= \frac{1 + 2400}{16} \\[6pt]
\left(y + \frac{1}{4}\right)^2 &= \frac{2401}{16} \\[6pt]
y + \frac{1}{4} &= \pm\frac{\sqrt{2401}}{\sqrt{16}}
  = \pm\frac{\sqrt{7^2 \cdot 7^2}}{4}
  = \pm\frac{49}{4} \\[6pt]
y &= \pm\frac{49}{4} - \frac{1}{4}
\end{aligned}
$$

The $\pm$ applies only to $\frac{49}{4}$, so split the two cases:

$$
\begin{aligned}
y_1 &= \frac{49}{4} - \frac{1}{4} = \frac{48}{4} = 12 \\[6pt]
y_2 &= -\frac{49}{4} - \frac{1}{4} = -\frac{50}{4} = -\frac{25}{2}
\end{aligned}
$$

**Step 4: find each $x$ with (1).**

$$
\begin{aligned}
y_1 = 12: \quad x + 12 &= 300 \ \Rightarrow \ x = 288 \\[6pt]
y_2 = -\tfrac{25}{2}: \quad x - \frac{25}{2} &= 300 \ \Rightarrow \ x = 300 + \frac{25}{2} = \frac{625}{2}
\end{aligned}
$$

**Check** against the problem statement:

| Pair | Add up to 300? | One is twice the square of the other? |
|---|---|---|
| $(288,\ 12)$ | $288 + 12 = 300$ $\checkmark$ | $2 \cdot 12^2 = 2 \cdot 144 = 288$ $\checkmark$ |
| $\left(\frac{625}{2},\ -\frac{25}{2}\right)$ | $\frac{625}{2} - \frac{25}{2} = \frac{600}{2} = 300$ $\checkmark$ | $2 \cdot \left(-\frac{25}{2}\right)^2 = 2 \cdot \frac{625}{4} = \frac{625}{2}$ $\checkmark$ |

The statement does not say the numbers are positive or whole, so both pairs are valid.

**Answer.** The numbers are $288$ and $12$, or $312.5$ and $-12.5$.

## Mistake / lesson

- **$\pm$ applies only to the root:** from $y + \frac{1}{4} = \pm\frac{49}{4}$ I wrote
  $y = \pm\frac{48}{4} = \pm 12$, as if the $\pm$ also covered $-\frac{1}{4}$. Split the cases:
  $\frac{49}{4} - \frac{1}{4}$ and $-\frac{49}{4} - \frac{1}{4}$ give $12$ and $-\frac{25}{2}$, not
  opposite numbers.
- **Check every pair:** the wrong pair $(312, -12)$ fails (2), since $2 \cdot (-12)^2 = 288 \ne 312$.
  A check would have caught it right away.
- **Don't discard solutions without a reason in the statement:** "two numbers" does not mean
  only one answer. A pair can be rejected only if it breaks a condition (e.g. "positive" or
  "whole numbers"), and this problem has none.

## Related

- [Systems of nonlinear equations and inequalities](../../../notes/algebra/nonlinear-systems/two-variables.md)
