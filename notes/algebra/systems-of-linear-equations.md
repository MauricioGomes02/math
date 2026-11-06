---
topics: [system-of-equations, linear-equation, substitution, elimination, inconsistent-system, dependent-system]
sources: [PRECALC 9.1]
---

# Systems of linear equations in two variables

## Definition

A **system of linear equations** is two or more linear equations in the same variables,
considered together:

$$
\begin{cases}
a_1 x + b_1 y = c_1 \\
a_2 x + b_2 y = c_2
\end{cases}
$$

A **solution** is an ordered pair $(x, y)$ that satisfies **every** equation at the same time.

## Intuition

Each equation is a line in the plane. Solving the system means finding the points that
lie on both lines. Two lines can relate in only three ways:

| Lines | Solutions | Name |
|---|---|---|
| Cross at one point (different slopes) | exactly one | **consistent, independent** |
| Parallel (same slope, different intercepts) | none | **inconsistent** |
| Same line | infinitely many | **consistent, dependent** |

## Methods

### 1. Graphing

Draw both lines and read off the intersection. Good for intuition, imprecise for
non-integer answers.

### 2. Substitution

1. Solve one equation for one variable (pick one with coefficient $1$ or $-1$ if possible).
2. Substitute that expression into the **other** equation and solve for the remaining variable.
3. Substitute back to find the first variable.
4. Check the pair in **both** original equations.

### 3. Addition (elimination)

1. Write both equations in the form $ax + by = c$.
2. Multiply one or both equations so one variable has opposite coefficients.
3. Add the equations; that variable cancels.
4. Solve, substitute back, check.

## Key results

**Recognizing the special cases while solving.** If a variable disappears and you get:

- a **false** statement such as $0 = 1$, the system is **inconsistent** (no solution);
- a **true** statement such as $0 = 0$, the system is **dependent** (infinitely many solutions).

**Writing a dependent solution.** Solve one equation for $y$ and write the set
$\{(x,\, y(x)) : x \in \mathbb{R}\}$. For example, for $x + 2y = 4$: $\left(x,\ 2 - \tfrac{1}{2}x\right)$.

## Common mistakes

- Substituting the expression back into the **same** equation it came from. You get $0=0$ and learn nothing.
- Multiplying only one side of an equation (or only some terms) when scaling for elimination.
- Fractions/decimals: clear them first (multiply by the LCD or by 10) to avoid arithmetic errors.
- Stopping after finding $x$; the solution is the **pair**.
- Not checking in **both** original equations.

## Exercises

| Exercise | Topic | Difficulty |
|---|---|---|
| [ex01](../../exercises/algebra/precalc-9.1-ex01.md) | Number of solutions | intro |
| [ex06](../../exercises/algebra/precalc-9.1-ex06.md) | Is the pair a solution? | intro |
| [ex07](../../exercises/algebra/precalc-9.1-ex07.md) | Is the pair a solution? | intro |
| [ex11](../../exercises/algebra/precalc-9.1-ex11.md) | Substitution | intro |
| [ex12](../../exercises/algebra/precalc-9.1-ex12.md) | Substitution | intermediate |
| [ex21](../../exercises/algebra/precalc-9.1-ex21.md) | Addition | intermediate |
| [ex25](../../exercises/algebra/precalc-9.1-ex25.md) | Addition | intermediate |
| [ex26](../../exercises/algebra/precalc-9.1-ex26.md) | Addition | intermediate |
| [ex56](../../exercises/algebra/precalc-9.1-ex56.md) | Break-even | intermediate |
| [ex19](../../exercises/algebra/precalc-9.1-ex19.md) | Substitution with fractions | hard |
| [ex27](../../exercises/algebra/precalc-9.1-ex27.md) | Addition with fractions | hard |
| [ex60](../../exercises/algebra/precalc-9.1-ex60.md) | Break-even price | hard |

## See also

- [Systems of linear equations in three variables](systems-of-linear-equations-three-variables.md)
- [Break-even analysis](../economics/break-even.md)
