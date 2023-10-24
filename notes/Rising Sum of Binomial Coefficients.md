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
$$\sum_{j\operatorname{=}0}^m\binom{n+j}n=\binom{n+m+1}{n+1}=\binom{n+m+1}m$$
$$\begin{aligned}
&\mathrm{If~}m\geq0\mathrm{~and~}n\geq1{:} \\
&\binom mm+\binom{m+1}m+\ldots+\binom{m+n}m=\binom{m+n+1}{m+1}.
\end{aligned}$$ 
#### Proof
$$\begin{aligned}
&\mathrm{If~}m\geq0\mathrm{~and~}n\geq1{:} \\
&\binom mm+\binom{m+1}m+\ldots+\binom{m+n}m=\binom{m+n+1}{m+1}. \\
&\rhd\binom{m+n+1}{m+1}=\binom{m+n}m+\binom{m+n}{m+1}= \\
&=\binom{m+n}m+(\binom{m+n-1}m+\binom{m+n-1}m)= \\
&=\binom{m+n}m+\binom{m+n-1}n+\ldots+\binom{m+1}{m+1}= \\
&=\binom{m+n}m+\binom{m+n-1}n+\ldots+\binom mm. \\
\end{aligned}$$



#### Sources:
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
$$\begin{aligned}
&\mathrm{If~}m\geq0\mathrm{~and~}n\geq1{:} \\
&\binom mm+\binom{m+1}m+\ldots+\binom{m+n}m=\binom{m+n+1}{m+1}.
\end{aligned}$$ 
Formula_additional:$$\begin{aligned}
&\mathrm{If~}m\geq0\mathrm{~and~}n\geq1{:} \\
&\binom mm+\binom{m+1}m+\ldots+\binom{m+n}m=\binom{m+n+1}{m+1}. \\
&\rhd\binom{m+n+1}{m+1}=\binom{m+n}m+\binom{m+n}{m+1}= \\
&=\binom{m+n}m+(\binom{m+n-1}m+\binom{m+n-1}m)= \\
&=\binom{m+n}m+\binom{m+n-1}n+\ldots+\binom{m+1}{m+1}= \\
&=\binom{m+n}m+\binom{m+n-1}n+\ldots+\binom mm. \\
\end{aligned}$$
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











