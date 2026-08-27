---
aliases: 
anki: false
created: 2024-04-24 17:13
parent:
  - "[[Discrete Random Variable]]"
  - "[[Distribution of r.v. MOC]]"
connected:
  - "[[Geometric distribution Geo(p) (discrete)]]"
tags:
---

> [!tip] Negative Binomial $\text{NB}(r, p)$ 
- [[PMF - p_X(x)|PMF]]: $p_X(x) = \binom{x+r-1}{r-1}p^r(1-p)^x$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = I_p(r, x+r-1)$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \frac{r(1-p)}{p}$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \frac{r(1-p)}{p^2}$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \left( \frac{p}{1-(1-p)e^s} \right)^r$  

