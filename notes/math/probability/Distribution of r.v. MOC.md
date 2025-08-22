---
aliases:
  - Распределение вероятностей в R
anki: false
created: 2023-10-29 19:46
parent:
  - "[[519.21  Probability theory]]"
  - "[[519.22 Statistic MOC]]"
connected:
  - "[[Distribution function]]"
tags:
  - content/moc
---

$\Omega=\mathbb{R}$ -  [[Sample space]] [[Real numbers R]]
$\mathcal{F}=\mathcal{B}(\mathbb{R})$ -  [[517.518.113 Borel sigma-algebra]]
P 一 [[Probability measure]] on $(\Omega,\mathcal{F})$ 一 ==distribution==

### 1.1 Discrete Distributions
- [[Uniform(a, b)  (discrete)]]
- [[Binomial distribution Bin(n, p)]]
    - [[Bernoulli(p)]]  
    - [[Poisson(lambda)]] 
    - [[Multinomial Mult(n, p)]]
    - [[Negative Binomial NB(r, p)]]
- [[Geometric distribution Geo(p) (discrete)]]
    - [[Hypergeometric Hyp(N, m, n)]]

### 1.2 Continuous Distributions
- [[Uniform(a, b)  (cont)]]
- [[Normal distribution]]
    - [[Log-Normal distribution]]
    - [[Multivariate Normal distribution]]
- Распределение максимума
- [[Student's distribution Student(v)]]
- [[Chi-square distribution]]
- [[F distribution]]
- [[Exponential distribution]]
- [[Gamma distribution]]
    - [[Inverse Gamma distribution]]
- [[Beta distribution]]
- [[Weibull distribution]]
- [[Pareto distribution]]
- [[Dirichlet distribution]]


[[Distribution comparing]]

# 7 Distribution Relationships

## Binomial

- $X_i \sim Bern(p)$ implies $\sum_{i=1}^{n} X_i \sim Bin(n, p)$
- $X \sim Bin(n, p)$ and $Y \sim Bin(m, p)$ implies $X + Y \sim Bin(n + m, p)$
- $\lim_{n \to \infty} Bin(n, p) = Po(np)$ when $n$ is large, $p$ is small
- $\lim_{n \to \infty} Bin(n, p) = \mathcal{N}(np, np(1 - p))$ when $n$ is large, $p$ far from 0 and 1

## Negative Binomial

- $X \sim NBin(1, p) = Geo(p)$
- $X \sim NBin(r, p)$ and $Y = \sum_{i=1}^{r} Geo(p)$ implies $X = Y$
- $X_i \sim NBin(r_i, p)$ implies $\sum X_i \sim NBin(\sum r_i, p)$
- $X \sim NBin(r, p)$ and $Y \sim Bin(s + r, p)$ implies $\mathbb{P}[X \leq s] = \mathbb{P}[Y \geq r]$

## Poisson

- $X_i \sim Po(\lambda_i)$ and $X_i \perp\!\!\!\perp X_j$ implies $\sum_{i=1}^{n} X_i \sim Po\left( \sum_{i=1}^{n} \lambda_i \right)$
- $X_i \sim Po(\lambda_i)$ and $X_i \perp\!\!\!\perp X_j$ implies $\sum X_i \sim Bin\left( n, \frac{\sum_{j=1}^{n} \lambda_j}{\sum_{j=1}^{n} \lambda_j} \right)$

## Exponential

- $X_i \sim Exp(\beta)$ and $X_i \perp\!\!\!\perp X_j$ implies $\sum_{i=1}^{n} X_i \sim Gamma(n, \beta)$
- Memoryless property: $\mathbb{P}[X > x + y | X > y] = \mathbb{P}[X > x]$
## Normal

- $X \sim \mathcal{N}(\mu, \sigma^2)$ implies $\left(\frac{X-\mu}{\sigma}\right) \sim \mathcal{N}(0, 1)$
- $X \sim \mathcal{N}(\mu, \sigma^2)$ and $Z = aX + b$ implies $Z \sim \mathcal{N}(a\mu + b, a^2\sigma^2)$
- $X_i \sim \mathcal{N}(\mu_i, \sigma_i^2)$ and $X_i \perp\!\!\!\perp X_j$ implies $\sum_i X_i \sim \mathcal{N}\left(\sum_i \mu_i, \sum_i \sigma_i^2\right)$
- $\mathbb{P}[a < X < b] = \Phi\left(\frac{b-\mu}{\sigma}\right) - \Phi\left(\frac{a-\mu}{\sigma}\right)$
- $\Phi(-x) = 1 - \Phi(x)$
- $\phi'(x) = -x\phi(x)$
- $\phi''(x) = (x^2 - 1)\phi(x)$
- Upper quantile of $\mathcal{N}(0, 1)$: $z_\alpha = \Phi^{-1}(1 - \alpha)$

## Gamma

- $X \sim Gamma(\alpha, \beta)$ is equivalent to $\frac{X}{\beta} \sim Gamma(\alpha, 1)$
- $Gamma(\alpha, \beta)$ is equivalent to $\sum_{i=1}^{\infty} Exp(\beta)$
- $X_i \sim Gamma(\alpha_i, \beta)$ and $X_i \perp\!\!\!\perp X_j$ implies $\sum_i X_i \sim Gamma\left(\sum_i \alpha_i, \beta\right)$
- $\frac{\Gamma(\alpha)}{\lambda^\alpha} = \int_{0}^{\infty} x^{\alpha-1} e^{-\lambda x} \, dx$

## Beta Distribution

- $\frac{1}{B(\alpha, \beta)} = \frac{\Gamma(\alpha + \beta)}{\Gamma(\alpha)\Gamma(\beta)} x^{\alpha-1}(1 - x)^{\beta-1}$
- $\mathbb{E}[X^k] = \frac{B(\alpha + k, \beta)}{B(\alpha, \beta)} = \frac{\alpha + k - 1}{\alpha + \beta + k - 1} \mathbb{E}[X^{k-1}]$
- $Beta(1, 1)$ is equivalent to $Unif(0, 1)$



![[Pasted image 20240423180438.png]]