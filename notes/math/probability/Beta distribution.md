---
aliases: 
publish: true
anki: false
created: 2024-04-24 13:32
parent:
  - "[[General Random Variables]]"
  - "[[Distribution of r.v. MOC]]"
connected: 
tags: 
---

> [!tip] Beta  $\text{Beta}(\alpha, \beta)$ 
> - [[PDF - f_X(x)|PDF]]: $f_X(x) = \frac{x^{\alpha-1}(1-x)^{\beta-1}}{B(\alpha, \beta)}$
> - [[CDF - F_X(x)|CDF]]: $F_X(x) = I_x(\alpha, \beta)$
> - [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \frac{\alpha}{\alpha + \beta}$
> - [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \frac{\alpha \beta}{(\alpha + \beta)^2(\alpha + \beta + 1)}$
> - [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = 1 + \sum_{k=1}^{\infty} \left( \prod_{r=0}^{k-1} \frac{\alpha + r}{\alpha + \beta + r} \right) \frac{s^k}{k!}$  

![[Pasted image 20240424154958.png|300]]
![[Pasted image 20240424154937.png|300]]