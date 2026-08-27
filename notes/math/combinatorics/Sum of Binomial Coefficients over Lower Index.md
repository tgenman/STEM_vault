---
aliases: 
anki: true
created: 2023-10-24 20:13
parent:
  - "[[Combinatorial identities]]"
connected: []
---

$$\sum_{i\operatorname{=}0}^n\binom ni=2^n$$
$$
\binom n0+\binom n1+\ldots+\binom nn=2^n.
$$
#### Proof
First
$$
2^n=(1+1)^n=\binom n01^n+\binom n11^{n-1}\cdot1+\\\ldots+\binom nn1^n=\binom n0+\binom n1+\ldots+\binom nn.
$$
Second:
$$2^n = \binom{n}{0} + \binom{n}{1} + \ldots + \binom{n}{n}.$$ 
How many subsets has an $n$-element set?

1) Multiplication rule: $2 \cdot 2 \cdot \ldots \cdot 2 = 2^n$.

2) The number of $k$-element subsets is $\binom{n}{k}$.

#### Source
- [Sum of Binomial Coefficients over Lower Index](https://proofwiki.org/wiki/Sum_of_Binomial_Coefficients_over_Lower_Index "Sum of Binomial Coefficients over Lower Index")


# Anki
TARGET DECK: math::combinatorics
START
Math_TWO_side
FRONT: Sum of Binomial Coefficients over Lower Index $\sum_{i\operatorname{=}0}^n\binom ni = \binom n0+\binom n1+\ldots+\binom nn =$
BACK: Sum of Binomial Coefficients over Lower Index $2^n =$
FORMULA:
ADDITIONAL:
ID: 1698168880304
END











