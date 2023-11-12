---
aliases: 
publish: true
anki: true
created: 2023-10-24 16:19
parent:
  - "[[Combinatorial identities]]"
connected:
  - "[[Binomial coefficient]]"
---
$$
\mathrm{If~} m \geq 0 \mathrm{~and~} n \geq 1{:}
\binom{m}{m} + \binom{m+1}{m} + \ldots + \binom{m+n}{m} = \binom{m+n+1}{m+1}.
$$

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


### Anki
TARGET DECK: Math::Combinatorics
START
Math prop
Question_eng: Rising Sum of Binomial Coefficients
Question_rus: 
Answer_eng: 
Answer_rus: 
Formula_main: $$\sum_{j\operatorname{=}0}^m\binom{n+j}n=\binom{n+m+1}{n+1}=\binom{n+m+1}m$$
If $m \geq 0$ and $n \geq 1$: $$\binom{m}{m} + \binom{m+1}{m} + \ldots + \binom{m+n}{m} = \binom{m+n+1}{m+1}.$$
Formula_additional:If ${} m \geq 0$ and $n \geq 1$:

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
<!--ID: 1698168880326-->
END


START
Math def
Title_eng: Rising Sum of Binomial Coefficients $$\sum_{j\operatorname{=}0}^m\binom{n+j}n=\binom mm+\binom{m+1}m+\ldots+\binom{m+n}m=  $$ 
Title_rus: 
Description_eng: Rising Sum of Binomial Coefficients
Description_rus: 
Formula_main: $$\binom{n+m+1}{n+1}=\binom{n+m+1}m $$
Formula_additional:
<!--ID: 1698168880333-->
END











