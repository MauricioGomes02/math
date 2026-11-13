---
source: PRECALC
ref: "9.3 #24"
topics: [system-of-equations, nonlinear-system, elimination, completing-the-square]
difficulty: intermediate
---

# Any method

## Problem

Solve the system using any method.

$$
\begin{cases}
x^2 + y^2 = 9 \\
y = 3 - x^2
\end{cases}
$$

## My attempt

**Label the equations.**

$$
\begin{aligned}
x^2 + y^2 &= 9 && (1) \ \text{circle, radius 3} \\
y &= 3 - x^2 && (2) \ \text{parabola, vertex } (0, 3) \text{, opens down}
\end{aligned}
$$

**What to expect.**

- Vertex $(0, 3)$ in (1): $0^2 + 3^2 = 9$, so the vertex is **on** the circle (one solution).
- Next point of the parabola, $x = 1$: $y = 3 - 1 = 2$. In (1): $1^2 + 2^2 = 5 < 9$, so it is
  **inside** the circle.
- The parabola enters the circle at the vertex and keeps going down, so it must leave once
  on each side: **3 solutions** expected.

**Step 1: write (2) in the same form as (1).**

$$
x^2 + y = 3 \qquad (2')
$$

**Step 2: (1) + (2') × (−1)** (the $x^2$ terms cancel)

$$
\begin{aligned}
x^2 + y^2 &= 9 \\
-x^2 - y &= -3 \\
\hline
y^2 - y &= 6
\end{aligned}
$$

**Step 3: complete the square.** $\left(-\frac{1}{2}\right)^2 = \frac{1}{4}$ on both sides:

$$
\begin{aligned}
y^2 - y + \frac{1}{4} &= \frac{25}{4} \\[6pt]
\left(y - \frac{1}{2}\right)^2 &= \frac{25}{4} \\[6pt]
y - \frac{1}{2} &= \pm\frac{5}{2} \\[6pt]
y &= \frac{1}{2} \pm \frac{5}{2} \ \Rightarrow \ y = 3 \ \text{or} \ y = -2
\end{aligned}
$$

**Step 4: find $x$ for each $y$** (substitute into (2), $x^2 = 3 - y$).

| $y$ | $x^2 = 3 - y$ | $x$ | Points |
|---|---|---|---|
| $3$ | $0$ | $0$ | $(0, 3)$ |
| $-2$ | $5$ | $\pm\sqrt{5}$ | $(\sqrt{5}, -2)$, $(-\sqrt{5}, -2)$ |

**Check in both original equations.** $(\sqrt{5}, -2)$ and $(-\sqrt{5}, -2)$ have the same
squares, so one row covers both.

| Point | (1): $x^2 + y^2$ | (2): $3 - x^2$ |
|---|---|---|
| $(0, 3)$ | $0 + 9 = 9 \ \checkmark$ | $3 - 0 = 3 = y \ \checkmark$ |
| $(\pm\sqrt{5}, -2)$ | $5 + 4 = 9 \ \checkmark$ | $3 - 5 = -2 = y \ \checkmark$ |

**Answer.** $(0, 3)$, $(\sqrt{5}, -2)$ and $(-\sqrt{5}, -2)$: three solutions, as expected.

## Mistake / lesson

- **Simplify as soon as a value appears.** I kept $y = \pm\frac{5}{2} + \frac{1}{2}$ until the
  end instead of $y = 3$ or $y = -2$, which made every later line heavier.
- **Try factoring before completing the square.** $y^2 - y - 6 = (y - 3)(y + 2)$: two numbers
  with product $-6$ and sum $-1$.
- **Inside the circle means $x^2 + y^2 < r^2$**, not "$y \le 3$". Use $<$: equality means
  **on** the circle.

## Related

- [Systems of nonlinear equations and inequalities](../../../notes/algebra/nonlinear-systems/two-variables.md)
- [PRECALC 9.3 #19](precalc-9.3-ex19.md) (circle and parabola)
