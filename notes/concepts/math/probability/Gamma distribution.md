---
aliases:
  - Гамма распределение
anki: false
created: 2024-04-24 13:32
parent:
  - "[[General Random Variables]]"
  - "[[Distribution of r.v. MOC]]"
connected:
tags:
---

> [!tip] Gamma  $\text{Gamma}(\alpha, \beta)$
- [[PDF - f_X(x)|PDF]]: $f_X(x) = \frac{\beta^{\alpha}x^{\alpha-1}e^{-\beta x}}{\Gamma(\alpha)}$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = \gamma\left(\alpha, \beta x\right) / \Gamma(\alpha)$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \frac{\alpha}{\beta}$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \frac{\alpha}{\beta^2}$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \left( \frac{1}{1-s/\beta} \right)^\alpha \quad \text{if} \quad s < \beta$

![[Pasted image 20240424143637.png|300]]
![[Pasted image 20240424143700.png|300]]

## параметры и связи

- $X \sim Gamma(\alpha, \beta)$ is equivalent to $\frac{X}{\beta} \sim Gamma(\alpha, 1)$
- $Gamma(\alpha, \beta)$ is equivalent to $\sum_{i=1}^{\infty} Exp(\beta)$
- $X_i \sim Gamma(\alpha_i, \beta)$ and $X_i \perp\!\!\!\perp X_j$ implies $\sum_i X_i \sim Gamma\left(\sum_i \alpha_i, \beta\right)$
- $\frac{\Gamma(\alpha)}{\lambda^\alpha} = \int_{0}^{\infty} x^{\alpha-1} e^{-\lambda x} \, dx$
