---
aliases: 
publish: true
anki: false
created: 2024-04-24 13:32
parent:
  - "[[General Random Variables]]"
  - "[[Distribution of r.v.]]"
connected: 
tags:
---

> [!tip] Inverse Gamma      $\text{InvGamma}(\alpha, \beta)$
> - [[PDF - f_X(x)|PDF]]: $f_X(x) = \frac{\beta^{\alpha}}{\Gamma(\alpha)} x^{-\alpha-1}e^{-\beta/x}$
> - [[CDF - F_X(x)|CDF]]: $F_X(x) = \frac{\Gamma(\alpha, \frac{\beta}{x})}{\Gamma(\alpha)}$
> - [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \frac{\beta}{\alpha - 1} \quad \text{if} \quad \alpha > 1$
> - [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \frac{\beta^2}{(\alpha - 1)^2(\alpha - 2)} \quad \text{if} \quad \alpha > 2$
> - [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \frac{2(-\beta s)^{\alpha/2} K_{\alpha}\left(\sqrt{-4\beta s}\right)}{\Gamma(\alpha)}$  

![[Pasted image 20240424144620.png|300]]
![[Pasted image 20240424144638.png|300]]