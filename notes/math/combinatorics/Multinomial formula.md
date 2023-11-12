---
aliases: 
publish: true
anki: false
created: 2023-11-11 23:47
parent: 
connected:
  - "[[Binomial theorem]]"
---

$$(x_1+x_2+\ldots+x_k)^n=\sum_{n_i\geq0,n_1+...+n_k=n}\binom{n}{n_1,n_2,...,n_k}x_1^{n_1}\cdots x_k^{n_k}$$


### Proof

The expression $(x_{1}+x_{2}+\ldots+x_{k})^{n}$ is the product of $n$ identical sums $$(x_{1}+x_{2}+\ldots+x_{k})\cdot\ldots\cdot(x_{1}+x_{2}+\ldots+x_{k}).$$ 

Expand all brackets and collect like terms. Terms will have the form $x_1^{n_1}\cdots x_k^{n_k}$ with $n_1+\ldots+n_k=n$ summing to $n$.

With the Multinomial formula, we prove that $(x_1+x_2+\ldots+x_k)^n$ is the product of $n$ sums: $$(x_1+x_2+\ldots+x_{k})\cdot\ldots\cdot(x_{1}+x_{2}+\ldots+x_{k}).$$ 
We obtain each term $x_1^{n_1}\cdots x_k^{n_k}$ by choosing $x_1$ in $n_1$ of the $n$ factors, $x_2$ in $n_2$, $x_3$ in $n_{3}$, and so on. Consequently, the coefficient of the monomial $x_1^{n_1}\cdots x_k^{n_k}$ is equal to the multinomial coefficient $\binom{n}{n_1,n_2,\ldots,n_k}$.






