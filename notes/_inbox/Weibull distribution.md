---
aliases: 
anki: false
created: 2024-04-24 13:32
parent:
  - "[[General Random Variables]]"
  - "[[Distribution of r.v. MOC]]"
connected: 
tags: 
---

> [!tip] Weibull $\text{Weibull}(\lambda, k)$ 
- [[PDF - f_X(x)|PDF]]: $f_X(x) = \frac{k}{\lambda} \left( \frac{x}{\lambda} \right)^{k-1}e^{-(x/\lambda)^k}$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = 1 - e^{-(x/\lambda)^k}$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \lambda \Gamma\left(1 + \frac{1}{k}\right)$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \lambda^2 \Gamma\left(1 + \frac{2}{k}\right) - \mu^2$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \sum_{n=0}^{\infty} \frac{s^n \lambda^n}{n!} \Gamma\left(1 + \frac{n}{k}\right)$  

![[Pasted image 20240424155737.png|300]]
![[Pasted image 20240424155757.png|300]]