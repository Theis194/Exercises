# Exercises

# 1.

Evaluate the following expressions and describe their derivation trees –use the big-step semantics of Aexp

1. $(\underline3 + \underline{12}) ∗ (\underline4 ∗ (\underline5 ∗ \underline8))$

$$\displaystyle\frac{
  \displaystyle\frac{\displaystyle\frac{\underline3\rarr 3\ \underline{12}\rarr 12}{\underline3 + \underline{12}\rarr 15}}{(\underline3 + \underline{12})\rarr 15}\displaystyle\frac{\displaystyle\frac{\underline4\rarr4}{\underline4 \rarr 4} \displaystyle\frac{\displaystyle\frac{\displaystyle\frac{\underline5 \rarr 5}{\underline5 \rarr 5}\displaystyle\frac{\underline8 \rarr 8}{\underline8 \rarr 8}}{\underline5 ∗ \underline8 \rarr 40}}{(\underline5 ∗ \underline8)\rarr 40}}  {(\underline4 ∗ (\underline5 ∗ \underline8))\rarr 160}}{(\underline3 + \underline{12}) ∗ (\underline4 ∗ (\underline5 ∗ \underline8))\rarr 2400}
$$

2. $(\underline3 + (\underline{12} ∗ \underline4)) ∗ (\underline5 ∗ \underline8)$

3. $(\underline3 + (\underline{12})) ∗ ((\underline4) ∗ (\underline5 ∗ \underline8))$
