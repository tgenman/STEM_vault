---
aliases: 
anki: true
created: 2023-10-24 16:19
parent:
  - "[[Combinatorial identities]]"
connected:
  - "[[Binomial coefficient]]"
  - "[[Sum of permutations for k classes]]"
---

$\mathrm{If~} m \geq 0 \mathrm{~and~} n \geq 1{:}$
$\sum_{j=0}^m\binom{n+j}n=\binom nn+\binom{n+1}n+\ldots+\binom{n+m}n = \binom{n+m+1}{n+1}$
$C_n^n + C_{n+1}^n + \ldots + C_{n+m}^n = C_{n+m+1}^{n+1}$
#### Proof
If $m \geq 0$ and $n \geq 1$:

$$
\binom{m}{m} + \binom{m+1}{m} + \ldots + \binom{m+n}{m} = \binom{m+n+1}{m+1}.
$$

To prove this, we can show that:

$$
\binom{m+n+1}{m+1} = \binom{m+n}{m} + \binom{m+n}{m+1}
$$

$$
= \binom{m+n}{m} + \left(\binom{m+n-1}{m} + \binom{m+n-1}{m+1}\right)
$$

$$
= \binom{m+n}{m} + \binom{m+n-1}{m+1} + \ldots + \binom{m+1}{m+1}
$$

$$
= \binom{m+n}{m} + \binom{m+n-1}{m+1} + \ldots + \binom{m}{m}.
$$


#### Bookmarks:
- [Rising Sum of Binomial Coefficients (wiki)](https://proofwiki.org/wiki/Rising_Sum_of_Binomial_Coefficients "Rising Sum of Binomial Coefficients")


# Anki
TARGET DECK: math::combinatorics
START
Math_TWO_side
TITLE: Rising Sum of Binomial Coefficients 
$\sum_{j=0}^m\binom{n+j}n=\binom nn+\binom{n+1}n+\ldots+\binom{n+m}n =$
DESCRIPTION: Rising Sum of Binomial Coefficients
$\binom{n+m+1}{n+1} =$
FORMULA: 
ADDITIONAL:
ID: 1698168880333
END











