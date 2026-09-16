---
aliases:
anki: false
created: 2024-04-24 17:13
parent:
  - "[[Discrete Random Variable]]"
  - "[[Distribution of r.v. MOC]]"
connected:
  - "[[Binomial distribution Bin(n, p)]]"
tags:
---

> [!tip] Negative Binomial $\text{NB}(r, p)$
- [[PMF - p_X(x)|PMF]]: $p_X(x) = \binom{x+r-1}{r-1}p^r(1-p)^x$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = I_p(r, x+r-1)$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \frac{r(1-p)}{p}$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \frac{r(1-p)}{p^2}$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \left( \frac{p}{1-(1-p)e^s} \right)^r$

## связи распределений

- $X \sim NBin(1, p) = Geo(p)$
- $X \sim NBin(r, p)$ and $Y = \sum_{i=1}^{r} Geo(p)$ implies $X = Y$
- $X_i \sim NBin(r_i, p)$ implies $\sum X_i \sim NBin(\sum r_i, p)$
- $X \sim NBin(r, p)$ and $Y \sim Bin(s + r, p)$ implies $\mathbb{P}[X \leq s] = \mathbb{P}[Y \geq r]$
