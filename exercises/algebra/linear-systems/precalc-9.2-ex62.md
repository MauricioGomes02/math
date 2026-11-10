---
source: PRECALC
ref: "9.2 #62"
topics: [system-of-equations, three-variables, word-problem, simple-interest]
difficulty: hard
---

# Three investments

## Problem

When his youngest child moved out, Deandre sold his home and made three investments using
gains from the sale. He invested \$80,500 into three accounts, one that paid 4% simple
interest, one that paid $3\frac{1}{8}\%$ simple interest, and one that paid $2\frac{1}{2}\%$
simple interest. He earned \$2,670 interest at the end of one year. If the amount of the
money invested in the second account was four times the amount invested in the third
account, how much was invested in each account?

## My attempt

**Model.** $x$ = amount in the 4% account, $y$ = amount in the $3\frac{1}{8}\%$ account,
$z$ = amount in the $2\frac{1}{2}\%$ account.

**Equation (1): total invested.**

$$
x + y + z = 80{,}500 \qquad (1)
$$

**Equation (2): total interest in one year.** Write the rates as fractions:
$3\frac{1}{8}\% = \frac{25/8}{100} = \frac{1}{32}$ and $2\frac{1}{2}\% = \frac{5/2}{100} = \frac{1}{40}$.

$$
\begin{aligned}
\frac{4}{100}x + \frac{25}{800}y + \frac{5}{200}z &= 2{,}670 \\[6pt]
\frac{1}{25}x + \frac{1}{32}y + \frac{1}{40}z &= 2{,}670 \\[6pt]
32x + 25y + 20z &= 2{,}136{,}000 && (2) \ \text{(× 800, the LCM)}
\end{aligned}
$$

**Equation (3): the second account is four times the third.**

$$
\begin{aligned}
y &= 4z \\
y - 4z &= 0 && (3)
\end{aligned}
$$

**Plan.** (3) has no $x$, so eliminate $x$ once from (1) and (2), then solve with (3).

**Step 1: (1) × (−32) + (2)**

$$
\begin{aligned}
-32x - 32y - 32z &= -2{,}576{,}000 \\
32x + 25y + 20z &= 2{,}136{,}000 \\
\hline
-7y - 12z &= -440{,}000 \\
7y + 12z &= 440{,}000 && (4)
\end{aligned}
$$

**Step 2: (3) × 3 + (4)** (makes $-12z$ and $+12z$)

$$
\begin{aligned}
3y - 12z &= 0 \\
7y + 12z &= 440{,}000 \\
\hline
10y &= 440{,}000 \\
y &= 44{,}000
\end{aligned}
$$

**Step 3: back-substitute.** $y = 44{,}000$ in (3):

$$
\begin{aligned}
44{,}000 - 4z &= 0 \\
z &= 11{,}000
\end{aligned}
$$

$y$ and $z$ in (1):

$$
\begin{aligned}
x + 44{,}000 + 11{,}000 &= 80{,}500 \\
x &= 25{,}500
\end{aligned}
$$

**Check every condition of the problem** with $(25{,}500,\ 44{,}000,\ 11{,}000)$:

| Condition | Substitution | Result |
|---|---|---|
| total is \$80,500 | $25{,}500 + 44{,}000 + 11{,}000$ | $80{,}500 \ \checkmark$ |
| interest is \$2,670 | $0.04(25{,}500) + 0.03125(44{,}000) + 0.025(11{,}000) = 1{,}020 + 1{,}375 + 275$ | $2{,}670 \ \checkmark$ |
| second is 4 × third | $4(11{,}000)$ | $44{,}000 \ \checkmark$ |

**Answer.** Deandre invested **\$25,500** at 4%, **\$44,000** at $3\frac{1}{8}\%$ and
**\$11,000** at $2\frac{1}{2}\%$.

## Mistake / lesson

- **"A is $k$ times B" means $A = k \cdot B$.** I wrote $4y = z$ (third = 4 × second) instead
  of $y = 4z$. Test with numbers: if the third has 1,000, the second must have 4,000.
- **Swapping an equation changes the answer, not just the order.** With $4y = z$ I got
  $(40{,}500,\ 8{,}000,\ 32{,}000)$; the correct values are all different.
- **Check against the statement, not against my own equations.** The first check used (1),
  (2), (3) as I wrote them, so a wrong (3) passed too (same lesson as [ex51](precalc-9.2-ex51.md)).

## Related

- [Systems of linear equations in three variables](../../../notes/algebra/linear-systems/three-variables.md)
- [PRECALC 9.2 #51](precalc-9.2-ex51.md) (word problem)
