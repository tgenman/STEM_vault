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

> [!tip] Negative binomial $\operatorname{NB}(r,p)$
> Here $X$ counts failures before the $r$-th success in independent Bernoulli trials: $r\in\mathbb N_{>0}$, $0<p\le1$.

- [[PMF - p_X(x)|PMF]]: $P(X=k)=\binom{k+r-1}{k}p^r(1-p)^k$, $k=0,1,\ldots$.
- [[CDF - F_X(x)|CDF]]: $F_X(x)=0$ for $x<0$; $F_X(x)=I_p(r,\lfloor x\rfloor+1)$ for $x\ge0$, where $I$ is the regularized incomplete beta function.
- [[Expected Value E(X)|Mean]]: $r(1-p)/p$.
- [[Variance V(X)|Variance]]: $r(1-p)/p^2$.
- [[Производящая функция моментов случайной M_X(s)|MGF]]: $M_X(s)=[p/(1-(1-p)e^s)]^r$, where $(1-p)e^s<1$.

## связи распределений

The local [[Geometric distribution Geo(p) (discrete)|Geo(p)]] counts trials from 1, so $X+1\sim\operatorname{Geo}(p)$ when $X\sim\operatorname{NB}(1,p)$.

For independent $G_i\sim\operatorname{Geo}(p)$, $\sum_{i=1}^rG_i-r\sim\operatorname{NB}(r,p)$. Independent $\operatorname{NB}(r_i,p)$ variables sum to $\operatorname{NB}(\sum_i r_i,p)$.

For integer $s\ge0$,
$$
P(X\le s)=P(Y\ge r),\qquad Y\sim\operatorname{Bin}(s+r,p).
$$
Both events describe reaching the $r$-th success within $s+r$ trials.

Source: [R stats: negative binomial](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/NegBinomial.html).
