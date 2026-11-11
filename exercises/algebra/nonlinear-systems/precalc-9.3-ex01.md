---
source: PRECALC
ref: "9.3 #1"
topics: [system-of-equations, nonlinear-system, proof]
difficulty: intro
---

# Can a nonlinear system have exactly two or three solutions?

## Problem

Explain whether a system of two nonlinear equations can have exactly two solutions. What about
exactly three? If not, explain why not. If so, give an example of such a system, in graph form,
and explain why your choice gives two or three answers.

## My attempt

**Yes to both:** a system of two nonlinear equations can have exactly two or exactly three
solutions.

**Why more than one is possible.** A linear equation has a constant slope, like the
arithmetic sequence $1, 3, 5, 7, \dots$ (always $+2$), so its graph is a line. A nonlinear
equation has terms such as $x^2$, $y^2$ or $xy$, so its graph is a **curve**:

- parabola
- circle
- ellipse

Two curves can bend and cross each other several times. For the curves of this section,
the number of solutions can be 0, 1, 2, 3 or 4.

**Example with exactly two: a circle and an ellipse.**

$$
\begin{aligned}
x^2 + y^2 &= 4 && (1) \ \text{circle, radius 2} \\
x^2 + 4y^2 &= 4 && (2) \ \text{ellipse, half-axes 2 and 1}
\end{aligned}
$$

The ellipse fits inside the circle and touches it only at its left and right ends.
Checking algebraically with (2) − (1):

$$
\begin{aligned}
3y^2 &= 0 \\
y &= 0 \\
x^2 &= 4 \ \Rightarrow \ x = \pm 2
\end{aligned}
$$

Solutions: $(2, 0)$ and $(-2, 0)$, exactly two.

**Example with exactly three: a circle and a parabola.**

$$
\begin{aligned}
x^2 + y^2 &= 1 && (1) \ \text{circle, radius 1} \\
y &= x^2 - 1 && (2) \ \text{parabola, vertex } (0, -1)
\end{aligned}
$$

The parabola's vertex **touches** the bottom of the circle, and its two arms **cross** the
circle at two more points. Checking algebraically, (2) gives $x^2 = y + 1$; substitute
into (1):

$$
\begin{aligned}
(y + 1) + y^2 &= 1 \\
y^2 + y &= 0 \\
y(y + 1) &= 0 \ \Rightarrow \ y = 0 \ \text{or} \ y = -1
\end{aligned}
$$

- $y = 0$: $x^2 = 1$, so $x = \pm 1$, giving $(1, 0)$ and $(-1, 0)$.
- $y = -1$: $x^2 = 0$, so $x = 0$, giving $(0, -1)$.

Solutions: $(1, 0)$, $(-1, 0)$ and $(0, -1)$, exactly three.

## Mistake / lesson

- **Answer every part of the question.** My first version answered "two" but skipped
  "exactly three".
- **An example means specific equations**, not just "a circle and an ellipse". Solving the
  example confirms the number of solutions.
- **"Nonlinear" is about the equation, not growth.** A circle doesn't "grow": it has two
  $y$ values for one $x$. Nonlinear means terms like $x^2$, $y^2$ or $xy$, so the graph is a
  curve.
- **Three solutions come from touching + crossing:** one tangent point plus two crossings.

## Related

- [Systems of nonlinear equations and inequalities](../../../notes/algebra/nonlinear-systems/two-variables.md)
