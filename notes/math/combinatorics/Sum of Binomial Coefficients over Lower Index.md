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
$$\begin{aligned}\\
&2^n=\binom n0+\binom n1+\ldots+\binom nn. \\
&\triangleright\textsf{How many subsets has an n-element} \\
&\text{set?} \\
&1)\text{ Multiplication rule. }2\cdotp2\cdotp...\cdotp2=2^n. \\
&\text{-} 2)The number of k-element subsets \\ is \binom nk.  
\end{aligned}$$

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
Formula_additional: $$\begin{aligned}\\
&2^n=\binom n0+\binom n1+\ldots+\binom nn. \\
&\triangleright\textsf{How many subsets has an n-element} \\
&\text{set?} \\
&1)\text{ Multiplication rule. }2\cdotp2\cdotp...\cdotp2=2^n. \\
&\text{-} 2)The number of k-element subsets \\ is \binom nk.  
\end{aligned}$$
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











