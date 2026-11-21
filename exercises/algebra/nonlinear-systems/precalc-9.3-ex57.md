---
source: PRECALC
ref: "9.3 #57"
topics: [nonlinear-system, profit, inequalities, word-problem]
difficulty: hard
---

# Profit range

## Problem

A laptop company has discovered their cost and revenue functions for each day:
$C(x) = 3x^2 - 10x + 200$ and $R(x) = -2x^2 + 100x + 50$. If they want to make a profit,
what is the range of laptops per day that they should produce? Round to the nearest number
which would generate profit.

## My attempt

**What to find.** Profit is revenue minus cost, $P(x) = R(x) - C(x)$. The company makes a
profit when $P(x) > 0$. The **break-even** points, where $P(x) = 0$, mark where the profit starts
and ends.

**Plan.** Build $P(x)$, solve $P(x) = 0$ by completing the square, decide on which side of the
roots $P(x) > 0$, then round to whole laptops that still give a profit.

**Step 1: build $P(x) = R(x) - C(x)$ and set it to $0$.**

$$
\begin{aligned}
(-2x^2 + 100x + 50) - (3x^2 - 10x + 200) &= 0 \\[6pt]
-2x^2 + 100x + 50 - 3x^2 + 10x - 200 &= 0 \\[6pt]
(-2x^2 - 3x^2) + (100x + 10x) + (50 - 200) &= 0 \\[6pt]
-5x^2 + 110x - 150 &= 0 && (1)
\end{aligned}
$$

So $P(x) = -5x^2 + 110x - 150$.

**Step 2: (1) ÷ (−5) and complete the square.** Half of $-22$ is $-11$, and $(-11)^2 = 121$,
so add $121 - 30$ to both sides:

$$
\begin{aligned}
x^2 - 22x + 30 &= 0 \\[6pt]
x^2 - 22x + 30 + (121 - 30) &= 0 + (121 - 30) \\[6pt]
x^2 - 22x + 121 &= 91 \\[6pt]
(x - 11)^2 &= 91 \\[6pt]
x - 11 &= \pm\sqrt{91} \\[6pt]
x &= 11 \pm \sqrt{91}
\end{aligned}
$$

With $\sqrt{91} \approx 9.54$ (between $9$ and $10$, since $81 < 91 < 100$):

$$
x_1 = 11 - \sqrt{91} \approx 1.46, \qquad x_2 = 11 + \sqrt{91} \approx 20.54
$$

**Step 3: where is the profit positive?** $P(x)$ has $-5x^2$, so its graph is a parabola that
opens **down**: below the axis before $x_1$ (loss), above the axis between the roots (profit),
below again after $x_2$ (loss). So $P(x) > 0$ for $1.46 < x < 20.54$.

**Step 4: round inward.** At the roots the profit is exactly $0$, and only whole laptops can be
produced. The lower end rounds **up** ($1.46 \to 2$) and the upper end rounds **down**
($20.54 \to 20$), so both stay inside the profit range.

**Check** with $P(x) = -5x^2 + 110x - 150$, at both ends and one step outside each:

| $x$ | Substitution | $P(x)$ | |
|---|---|---|---|
| $1$ | $-5(1) + 110(1) - 150$ | $-45$ | loss |
| $2$ | $-5(4) + 110(2) - 150$ | $50$ | profit $\checkmark$ |
| $20$ | $-5(400) + 110(20) - 150$ | $50$ | profit $\checkmark$ |
| $21$ | $-5(441) + 110(21) - 150$ | $-45$ | loss |

The values are symmetric because the parabola is symmetric about its vertex at $x = 11$.

**Answer.** The company should produce between **2 and 20 laptops per day**.

## Mistake / lesson

- **Copy from the statement:** I wrote $R(x)$ with $+5$ instead of $+50$. Copy each function
  from the problem statement, not from memory or the previous line, and compare term by term.
- **Square of the half-coefficient:** I wrote $(-11)^2 = 141$. It is $121$. Check the number
  added when completing the square: $x^2 - 22x + 121$ must factor as $(x - 11)^2$.
- **The answer is a range, rounded inward:** the break-even points are where profit is $0$, so
  the answer is the interval between them. Rounding the upper end up ($21$) lands in the loss
  zone: $P(21) = -45$. Lower end rounds up, upper end rounds down.

## Related

- [Systems of nonlinear equations and inequalities](../../../notes/algebra/nonlinear-systems/two-variables.md)
- [Break-even analysis](../../../notes/economics/break-even.md)
