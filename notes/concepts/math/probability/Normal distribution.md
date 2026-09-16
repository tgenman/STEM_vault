---
aliases:
  - Нормальное распределение
anki: true
created: 2024-01-06 13:03
parent:
  - "[[Distribution of r.v. MOC]]"
  - "[[General Random Variables]]"
connected:
  - "[[519.21  Probability theory]]"
  - "[[Стандартное нормальное распределение]]"
tags:
---

> [!tip] Normal $\mathcal{N}(\mu, \sigma^2)$
- [[PDF - f_X(x)|PDF]]: $\phi(x) = \frac{1}{\sqrt{2\pi}\sigma} e^{-\frac{(x-\mu)^2}{2\sigma^2}}$
- [[CDF - F_X(x)|CDF]]: $\Phi(x) = \frac{1}{\sqrt{2\pi}\sigma} \int_{-\infty}^x e^{-\frac{(t-\mu)^2}{2\sigma^2}} dt$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \mu$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \sigma^2$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \exp\left\{ \mu s + \frac{\sigma^2 s^2}{2} \right\}$


![[Pasted image 20240424114504.png|300]]
![[Pasted image 20240424114536.png|300]]


## связи распределений

- $X \sim \mathcal{N}(\mu, \sigma^2)$ implies $\left(\frac{X-\mu}{\sigma}\right) \sim \mathcal{N}(0, 1)$
- $X \sim \mathcal{N}(\mu, \sigma^2)$ and $Z = aX + b$ implies $Z \sim \mathcal{N}(a\mu + b, a^2\sigma^2)$
- $X_i \sim \mathcal{N}(\mu_i, \sigma_i^2)$ and $X_i \perp\!\!\!\perp X_j$ implies $\sum_i X_i \sim \mathcal{N}\left(\sum_i \mu_i, \sum_i \sigma_i^2\right)$
- $\mathbb{P}[a < X < b] = \Phi\left(\frac{b-\mu}{\sigma}\right) - \Phi\left(\frac{a-\mu}{\sigma}\right)$

# Anki
TARGET DECK: math::probability
START
math_complex
FRONT: Normal distribution $\mathcal{N}(\mu, \sigma^2)$
BACK:
- [[PDF - f_X(x)|PDF]]: $\phi(x) = \frac{1}{\sqrt{2\pi}\sigma} e^{-\frac{(x-\mu)^2}{2\sigma^2}}$
- [[CDF - F_X(x)|CDF]]: $\Phi(x) = \frac{1}{\sqrt{2\pi}\sigma} \int_{-\infty}^x e^{-\frac{(t-\mu)^2}{2\sigma^2}} dt$$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \mu$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \sigma^2$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \exp\left\{ \mu s + \frac{\sigma^2 s^2}{2} \right\}$
FORMULA:
ADDITIONAL:
PICTURE:
![[Pasted image 20240424114504.png|300]]
![[Pasted image 20240424114536.png|300]]
ID: 1713948403543
END
