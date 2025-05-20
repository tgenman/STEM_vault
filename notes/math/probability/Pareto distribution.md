---
aliases: 
anki: false
created: 2024-04-24 13:32
parent:
  - "[[General Random Variables]]"
  - "[[Distribution of r.v. MOC]]"
connected:
  - "[[👤Pareto, Vilfredo|Pareto]]"
tags: 
---

> [!tip] Pareto $\text{Pareto}(x_m, \alpha)$     
- [[PDF - f_X(x)|PDF]]: $f_X(x) = \frac{\alpha x_m^\alpha}{x^{\alpha + 1}} \quad x \ge x_m$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = 1 - \left(\frac{x_m}{x}\right)^\alpha \quad x \ge x_m$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \frac{\alpha x_m}{\alpha - 1} \quad \text{if} \quad \alpha > 1$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \frac{\alpha x_m^2}{(\alpha - 1)^2(\alpha - 2)} \quad \text{if} \quad \alpha > 2$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \alpha (-x_{m}s)^{\alpha}\Gamma(-\alpha, -x_{m}s)^{-\alpha} \quad \text{if} \quad s < 0$  

![[Pasted image 20240424160338.png|300]]

![[Pasted image 20240424160354.png|300]]