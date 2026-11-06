---
topics: [system-of-equations, three-variables, elimination, inconsistent-system, dependent-system]
sources: [PRECALC 9.2]
---

# Systems of linear equations in three variables

## Definition

A system of three linear equations in three variables:

$$
\begin{cases}
a_1 x + b_1 y + c_1 z = d_1 \\
a_2 x + b_2 y + c_2 z = d_2 \\
a_3 x + b_3 y + c_3 z = d_3
\end{cases}
$$

A **solution** is an ordered triple $(x, y, z)$ that satisfies **every** equation at the same time.

## Intuition

Each equation is a **plane** in space. Solving the system means finding the points that lie
on all three planes.

| Planes | Solutions | Name |
|---|---|---|
| Meet at a single point | exactly one | **consistent, independent** |
| No point common to all three (e.g. parallel planes) | none | **inconsistent** |
| Meet along a line, or are the same plane | infinitely many | **consistent, dependent** |

## Method: elimination

The idea is to reduce the system to one you already know how to solve (two variables).

1. Pick **two** equations and eliminate one variable (say $x$). You get equation (A) in $y, z$.
2. Pick a **different** pair (it must use the equation left out in step 1) and eliminate the
   **same** variable. You get equation (B) in $y, z$.
3. Solve the $2 \times 2$ system (A), (B).
4. Substitute back into one of the original equations to find the eliminated variable.
5. Check the triple in **all three** original equations.

If an equation already lacks a variable, use it: you only need to eliminate that variable
from one other pair.

## Key results

- A **false** statement ($0 = c$, $c \neq 0$) while eliminating means **no solution**.
- A **true** statement ($0 = 0$) means the equations are not independent: **infinitely many**
  solutions. Write the solution in terms of one or two free variables.

## Common mistakes

- Eliminating **different** variables in the two pairs, which leaves a system that is still
  in three variables.
- Using the same pair of equations twice, so the third equation is never used.
- Fractions/decimals: clear them first (multiply by the LCD or by a power of 10).
- Checking only one equation.

## Exercises

| Exercise | Topic | Difficulty |
|---|---|---|
| [ex01](../../exercises/algebra/precalc-9.2-ex01.md) | Number of solutions | intro |
| [ex06](../../exercises/algebra/precalc-9.2-ex06.md) | Is the triple a solution? | intro |
| [ex11](../../exercises/algebra/precalc-9.2-ex11.md) | Elimination | intermediate |
| [ex17](../../exercises/algebra/precalc-9.2-ex17.md) | Elimination with a missing variable | intermediate |
| [ex20](../../exercises/algebra/precalc-9.2-ex20.md) | Elimination | intermediate |
| [ex23](../../exercises/algebra/precalc-9.2-ex23.md) | Elimination | intermediate |
| [ex51](../../exercises/algebra/precalc-9.2-ex51.md) | Word problem | intermediate |
| [ex30](../../exercises/algebra/precalc-9.2-ex30.md) | Elimination with fractions | hard |
| [ex37](../../exercises/algebra/precalc-9.2-ex37.md) | Elimination with decimals | hard |
| [ex46](../../exercises/algebra/precalc-9.2-ex46.md) | Elimination with shifted variables | hard |
| [ex62](../../exercises/algebra/precalc-9.2-ex62.md) | Investments | hard |

## See also

- [Systems of linear equations in two variables](systems-of-linear-equations.md)
