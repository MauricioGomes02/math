---
topics: [system-of-equations, nonlinear-system, substitution, elimination, inequalities, feasible-region]
sources: [PRECALC 9.3]
---

# Systems of nonlinear equations and inequalities in two variables

## Definition

A **nonlinear system** is a system where at least one equation is not linear: it has a
term such as $x^2$, $y^2$, $xy$ or $\frac{1}{y}$. For example:

$$
\begin{cases}
x - y = 1 \\
x^2 + y^2 = 25
\end{cases}
$$

A **solution** is an ordered pair $(x, y)$ that satisfies **every** equation.

## Intuition

Each equation is a curve (line, circle, parabola, ellipse, hyperbola). The solutions are the
points where the curves cross. Unlike two lines, curves can cross **more than once**:

| Curves | Possible number of solutions |
|---|---|
| line and circle | 0, 1 or 2 |
| line and parabola | 0, 1 or 2 |
| circle and parabola | 0, 1, 2, 3 or 4 |
| circle and ellipse | 0, 1, 2, 3 or 4 |

Sketching the two curves first tells you how many solutions to expect.

## Methods

### 1. Substitution

Best when one equation is linear or easy to solve for a variable.

1. Solve the simpler equation for one variable.
2. Substitute into the other equation. You usually get a **quadratic**: solve it
   (factor or use the quadratic formula).
3. For **each** value found, substitute back to get the partner value.
4. Check every pair in **both** original equations.

### 2. Elimination

Best when both equations have $x^2$ and $y^2$ (and no other $x$, $y$ terms). Treat $x^2$ and
$y^2$ as the "variables" and eliminate one of them, as in a linear system.

1. Multiply so one squared term has opposite coefficients, and add.
2. Solve for the remaining square, e.g. $x^2 = 9$, so $x = \pm 3$.
3. Substitute back to find the other square, then take $\pm$ roots.
4. Combine signs into pairs and check each pair.

## Key results

- **Square roots give two values:** $x^2 = k$ with $k > 0$ means $x = \sqrt{k}$ **or**
  $x = -\sqrt{k}$.
- **Reject impossible values:** $x^2 = k$ with $k < 0$ has no real solution, so that branch
  gives no points.
- **Pairs, not lists:** each solution is a pair $(x, y)$. With $x = \pm a$ and $y = \pm b$
  from elimination, write all valid combinations, e.g. $(a, b), (a, -b), (-a, b), (-a, -b)$.

## Systems of inequalities

1. Graph each boundary curve: **dashed** for $<$ or $>$, **solid** for $\le$ or $\ge$.
2. Pick a test point not on the curve (often $(0, 0)$) to decide which side to shade.
3. The solution set (**feasible region**) is where all shadings overlap.
4. Find the intersection points of the boundaries by solving the system of equations.

## Common mistakes

- Forgetting the $\pm$ when taking a square root.
- Substituting back into the **squared** equation and getting extra pairs that fail the
  other equation. Substitute into the simpler (linear) one when possible.
- Pairing an $x$ with the wrong $y$.
- Keeping a value that makes $y^2$ or $x^2$ negative.
- Checking in only one equation.

## Exercises

| Exercise | Topic | Difficulty |
|---|---|---|
| [ex01](../../../exercises/algebra/nonlinear-systems/precalc-9.3-ex01.md) | Number of solutions | intro |
| [ex09](../../../exercises/algebra/nonlinear-systems/precalc-9.3-ex09.md) | Substitution | intro |
| [ex06](../../../exercises/algebra/nonlinear-systems/precalc-9.3-ex06.md) | Substitution | intermediate |
| [ex14](../../../exercises/algebra/nonlinear-systems/precalc-9.3-ex14.md) | Elimination | intermediate |
| [ex19](../../../exercises/algebra/nonlinear-systems/precalc-9.3-ex19.md) | Any method | intermediate |
| [ex24](../../../exercises/algebra/nonlinear-systems/precalc-9.3-ex24.md) | Any method | intermediate |
| [ex30](../../../exercises/algebra/nonlinear-systems/precalc-9.3-ex30.md) | Any method | intermediate |
| [ex41](../../../exercises/algebra/nonlinear-systems/precalc-9.3-ex41.md) | System of inequalities | intermediate |
| [ex55](../../../exercises/algebra/nonlinear-systems/precalc-9.3-ex55.md) | Word problem | intermediate |
| [ex38](../../../exercises/algebra/nonlinear-systems/precalc-9.3-ex38.md) | Any method | hard |
| [ex52](../../../exercises/algebra/nonlinear-systems/precalc-9.3-ex52.md) | Any method | hard |
| [ex57](../../../exercises/algebra/nonlinear-systems/precalc-9.3-ex57.md) | Profit range | hard |

## See also

- [Systems of linear equations in two variables](../linear-systems/two-variables.md)
- [Break-even analysis](../../economics/break-even.md)
