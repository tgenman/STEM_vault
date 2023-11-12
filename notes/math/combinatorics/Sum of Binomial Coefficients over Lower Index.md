---
aliases: 
publish: true
anki: true
created: 2023-10-24 20:13
parent:
  - "[[Combinatorial identities]]"
connected: []
---
$$
\sum_{i\operatorname{=}0}^n\binom ni=2^n
$$
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


### Anki
TARGET DECK: Math::Combinatorics
START
Math prop
Question_eng: Sum of Binomial Coefficients over Lower Index
Question_rus: 
Answer_eng: 
Answer_rus: 
Formula_main: $$
\sum_{i\operatorname{=}0}^n\binom ni=2^n
$$
$$
\binom n0+\binom n1+\ldots+\binom nn=2^n.
$$
Formula_additional: The expression $2^n = \binom{n}{0} + \binom{n}{1} + \ldots + \binom{n}{n}$ denotes that the power of two is equal to the sum of binomial coefficients for a given $n$.

How many subsets has an $n$-element set?

1) By the multiplication rule, multiplying $2 \cdot 2 \cdot \ldots \cdot 2$ (n times), we obtain $2^n$.

2) The number of $k$-element subsets is $\binom{n}{k}$.
<!--ID: 1698168880293-->
END


START
Math def
Title_eng: Sum of Binomial Coefficients over Lower Index $$
\sum_{i\operatorname{=}0}^n\binom ni = \binom n0+\binom n1+\ldots+\binom nn =
$$ 
Title_rus: 
Description_eng: Sum of Binomial Coefficients over Lower Index
Description_rus: 
Formula_main: $$
=2^n
$$
Formula_additional:
<!--ID: 1698168880304-->
END











