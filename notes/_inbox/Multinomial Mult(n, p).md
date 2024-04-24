---
aliases: 
publish: true
anki: false
created: 2024-04-24 17:13
parent:
  - "[[Discrete Random Variable]]"
  - "[[Distribution of r.v. MOC]]"
connected:
  - "[[Binomial distribution Bin(n, p)]]"
tags:
---

> [!tip] Multinomial       | $\text{Mult}(n, p)$ 
> - [[PMF - p_X(x)|PMF]]: $p_X(x) = \frac{n!}{x_1!\ldots x_k!}p_1^{x_1}\ldots p_k^{x_k} \text{ } \sum_{i=1}^k x_i = n$
> - [[CDF - F_X(x)|CDF]]: not
> - [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \begin{pmatrix} np_1 \\ \vdots \\ np_k \end{pmatrix}$
> - [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \begin{pmatrix} np_1(1 - p_1) & -np_1p_2 \\ -np_2p_1 & \ddots \\\end{pmatrix}$
> - [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \left( \sum_{i=0}^k p_ie^{s_i} \right)^n$  


