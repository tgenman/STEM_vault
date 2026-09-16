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

Here $\alpha>0$ is shape and $\beta>0$ is rate, with scale $1/\beta$. The density is defined for $x>0$ and zero for $x<0$; its limiting value at zero depends on shape.

- If $X\sim\operatorname{Gamma}(\alpha,\text{rate}=\beta)$, then $\beta X\sim\operatorname{Gamma}(\alpha,\text{rate}=1)$.
- Mutually independent $\operatorname{Gamma}(\alpha_i,\text{rate}=\beta)$ variables sum to $\operatorname{Gamma}(\sum_i\alpha_i,\text{rate}=\beta)$.
- For integer $n\ge1$, a sum of $n$ independent exponentials of rate $\beta$ is $\operatorname{Gamma}(n,\text{rate}=\beta)$; this is a finite sum.
- For $\alpha,\lambda>0$:
$$
\int_0^\infty x^{\alpha-1}e^{-\lambda x}\,dx=\frac{\Gamma(\alpha)}{\lambda^\alpha}.
$$

Sources: [R stats: Gamma](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/GammaDist.html), [sums and MGFs](https://heogden.github.io/math2011/sums-of-random-variables.html).
