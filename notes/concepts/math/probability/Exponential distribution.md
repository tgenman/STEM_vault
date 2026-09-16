---
aliases: 
anki: false
created: 2024-04-24 13:28
parent:
  - "[[Distribution of r.v. MOC]]"
  - "[[General Random Variables]]"
connected: 
tags: []
---

> [!tip] Exponential  distribution  $\text{Exp}(\beta)$, where $\beta = \frac{1}{\lambda}$
- $\lambda$ - rate
- [[PDF - f_X(x)|PDF]]: $f_X(x) = \frac{1}{\beta}e^{-x/\beta}$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = 1 - e^{-x/\beta}$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \beta$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \beta^2$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \frac{1}{1-s\beta} \quad \text{if} \quad s < \frac{1}{\beta}$  


![[Pasted image 20240424133126.png|300]]
![[Pasted image 20240424133102.png|300]]

## параметры и связи

Here $\beta>0$ is scale (mean), and $\lambda=1/\beta$ is rate. The density and CDF formulas apply to $x\ge0$; both are zero for $x<0$.

For mutually independent $X_i\sim\operatorname{Exp}(\text{scale}=\beta)$,
$$
\sum_{i=1}^nX_i\sim\operatorname{Gamma}(\text{shape}=n,\text{rate}=1/\beta).
$$
This uses the rate convention of [[Gamma distribution]].

For $x,y\ge0$,
$$
P(X>x+y\mid X>y)=P(X>x).
$$

Sources: [R stats: exponential](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/Exponential.html), [distribution relationships](https://www.statlect.com/probability-distributions/relationships-among-probability-distributions).
