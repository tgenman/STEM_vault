---
aliases:
  - Распределение вероятностей в R
publish: true
anki: false
created: 2023-10-29 19:46
parent:
  - "[[519.21  Probability theory]]"
  - "[[519.22 Statistic MOC]]"
connected:
  - "[[Distribution function]]"
tags:
  - empty
---

$\Omega=\mathbb{R}$ -  [[Sample space]] [[Real numbers R]]
$\mathcal{F}=\mathcal{B}(\mathbb{R})$ -  [[517.518.113 Borel sigma-algebra]]
P 一 [[Probability measure]] on $(\Omega,\mathcal{F})$ 一 ==distribution==

![[Pasted image 20240423180438.png]]

### 1.1 Discrete Distributions

| Distribution                  | Notation                      | $F_X(x)$                                                                              | $f_X(x)$                                              | $\mathbb{E}[X]$        | $\text{Var}[X]$                                                                                                                                                                       | $M_X(s)$                                   |
| ----------------------------- | ----------------------------- | ------------------------------------------------------------------------------------- | ----------------------------------------------------- | ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| [[Uniform(a, b)  (discrete)]] | $\text{Unif}\{a, \ldots, b\}$ | $\begin{cases} 0 & x < a \\ \frac{x-a}{b-a} & a \le x \le b \\ 1 & x > b \end{cases}$ | $\frac{1}{b-a} \mathbb{I}(a \le x \le b)$             | $\frac{a+b}{2}$        | $\frac{(b-a+1)^2-1}{12}$                                                                                                                                                              | $\frac{e^{as} - e^{(b+1)s}}{s(b-a)}$       |
| [[Bernoulli(p)]]              | $\text{Bern}(p)$              | $(1-p)^{1-x}$                                                                         | $p^x(1-p)^{1-x}$                                      | $p$                    | $p(1-p)$                                                                                                                                                                              | $1-p+pe^s$                                 |
| [[Binomial Bin(n, p)]]            | $\text{Bin}(n, p)$            | $I_{1-p}(n-x, x+1)$                                                                   | $\binom{n}{x}p^x(1-p)^{n-x}$                          | $np$                   | $np(1-p)$                                                                                                                                                                             | $(1-p+pe^s)^n$                             |
| Multinomial                   | $\text{Mult}(n, p)$           | -                                                                                     | $\frac{n!}{x_1!\ldots x_k!}p_1^{x_1}\ldots p_k^{x_k}$ | $\sum_{i=1}^k x_i = n$ | $\begin{pmatrix}np_1 & -np_1p_2 & \cdots & -np_1p_k \\ -np_2p_1 & np_2 & \cdots & -np_2p_k \\ \vdots & \vdots & \ddots & \vdots \\ -np_kp_1 & -np_kp_2 & \cdots & np_k \end{pmatrix}$ | $\left( \sum_{i=0}^k p_ie^{s_i} \right)^n$ |
| Hypergeometric                | $\text{Hyp}(N, m, n)$         | $\approx \Phi \left( \frac{x-np}{\sqrt{np(1-p)}} \right)$                             | $\frac{\binom{m}{x} \binom{N-m}{n-x}}{\binom{N}{n}}$  | $\frac{nm}{N}$         | $\frac{nm(N-n)(N-m)}{N^2(N-1)}$                                                                                                                                                       | -                                          |
| Negative Binomial             | $\text{NB}(r, p)$             | $I_p(r, x+r-1)$                                                                       | $\binom{x+r-1}{r-1}p^r(1-p)^x$                        | $\frac{r(1-p)}{p}$     | $\frac{r(1-p)}{p^2}$                                                                                                                                                                  | $\left( \frac{p}{1-(1-p)e^s} \right)^r$    |
| [[Geometric(p) (discrete)]]   | $\text{Geo}(p)$               | $1-(1-p)^x \quad x \in \mathbb{N}^+$                                                  | $p(1-p)^{x-1} \quad x \in \mathbb{N}^+$               | $\frac{1}{p}$          | $\frac{1-p}{p^2}$                                                                                                                                                                     | $\frac{pe^s}{1-(1-p)e^s}$                  |
| [[Poisson(lambda)]]           | $\text{Po}(\lambda)$          | $e^{-\lambda}\sum_{i=0}^x \frac{\lambda^i}{i!}$                                       | $\frac{\lambda^x e^{-\lambda}}{x!}$                   | $\lambda$              | $\lambda$                                                                                                                                                                             | $e^{\lambda(e^s-1)}$                       |

### 1.2 Continuous Distributions

| Distribution | Notation | $F_X(x)$ | $f_X(x)$ | $\mathbb{E}[X]$ | $\text{Var}[X]$ | $M_X(s)$ |
|--------------|----------|----------|----------|-----------------|-----------------|-----------|
| Uniform | $\text{Unif}(a, b)$ | $\begin{cases} 0 & x < a \\ \frac{x-a}{b-a} & a \le x < b \\ 1 & x > b \end{cases}$ | $\frac{1}{b-a} \mathbb{I}(a \le x < b)$ | $\frac{a+b}{2}$ | $\frac{(b-a)^2}{12}$ | $e^{sb} - e^{sa} \over s(b-a)$ |
| Normal | $\mathcal{N}(\mu, \sigma^2)$ | $\phi(x) = \frac{1}{\sqrt{2\pi}\sigma} \int_{-\infty}^x e^{-\frac{(t-\mu)^2}{2\sigma^2}} dt$ | $\phi(x) = \frac{1}{\sqrt{2\pi}\sigma} e^{-\frac{(x-\mu)^2}{2\sigma^2}}$ | $\mu$ | $\sigma^2$ | $\exp\left\{ \mu s + \frac{\sigma^2 s^2}{2} \right\}$ |
| Log-Normal | $\text{ln}\mathcal{N}(\mu, \sigma^2)$ | $\frac{1}{2} + \frac{1}{2} \text{erf}\left(\frac{\ln x - \mu}{\sqrt{2\sigma^2}}\right)$ | $\frac{1}{x\sqrt{2\pi\sigma^2}} e^{-\frac{(\ln x - \mu)^2}{2\sigma^2}}$ | $e^{\mu+\frac{\sigma^2}{2}}$ | $(e^{\sigma^2} - 1)e^{2\mu+\sigma^2}$ | - |
| Multivariate Normal | $\text{MVN}(\mu, \Sigma)$ | - | $(2\pi)^{-k/2}|\Sigma|^{-1/2}e^{-\frac{1}{2}(x-\mu)^{\text{T}}\Sigma^{-1}(x-\mu)}$ | $\mu$ | $\Sigma$ | $\exp\left\{ \mu^{\text{T}} s + \frac{1}{2} s^{\text{T}} \Sigma s \right\}$ |
| Student's $t$ | $\text{Student}(v)$ | $I_x\left(\frac{v}{2}, \frac{v}{2}\right)$ | $\frac{\Gamma(\frac{v+1}{2})}{\sqrt{v\pi}\Gamma(\frac{v}{2})}(1 + \frac{x^2}{v})^{-\frac{v+1}{2}}$ | $0 \quad \text{if} \quad v > 1$ | $\frac{v}{v - 2} \quad \text{if} \quad v > 2$ | - |
| Chi-square | $\chi^2_k$ | $\frac{1}{\Gamma(k/2)} \gamma\left(\frac{k}{2}, \frac{x}{2}\right)$ | $\frac{x^{k/2-1}e^{-x/2}}{2^k\Gamma(k/2)}$ | $k$ | $2k$ | $(1 - 2s)^{-k/2} \quad \text{if} \quad s < 1/2$ |
| F | $F(d_1, d_2)$ | $I_{\frac{d_1x}{d_1x + d_2}}\left(\frac{d_1}{2}, \frac{d_2}{2}\right)$ | $\frac{\sqrt{\frac{(d_1x)^{d_1}d_2^{d_2}}{(d_1x+d_2)^{d_1+d_2}}}}{xB\left(\frac{d_1}{2}, \frac{d_2}{2}\right)}$ | $\frac{d_2}{d_2 - 2} \quad \text{if} \quad d_2 > 2$ | - | - |
| Exponential | $\text{Exp}(\beta)$ | $1 - e^{-x/\beta}$ | $\frac{1}{\beta}e^{-x/\beta}$ | $\beta$ | $\beta^2$ | $\frac{1}{1-s\beta} \quad \text{if} \quad s < \frac{1}{\beta}$ |
| Gamma | $\text{Gamma}(\alpha, \beta)$ | $\gamma\left(\alpha, \beta x\right) / \Gamma(\alpha)$ | $\frac{\beta^{\alpha}x^{\alpha-1}e^{-\beta x}}{\Gamma(\alpha)}$ | $\frac{\alpha}{\beta}$ | $\frac{\alpha}{\beta^2}$ | $\left( \frac{1}{1-s/\beta} \right)^\alpha \quad \text{if} \quad s < \beta$ |
| Inverse Gamma | $\text{InvGamma}(\alpha, \beta)$ | - | $\frac{\beta^{\alpha}}{\Gamma(\alpha)} x^{-\alpha-1}e^{-\beta/x}$ | $\frac{\beta}{\alpha - 1} \quad \text{if} \quad \alpha > 1$ | $\frac{\beta^2}{(\alpha - 1)^2(\alpha - 2)} \quad \text{if} \quad \alpha > 2$ | - |
| Dirichlet | $\text{Dir}(\alpha)$ | - | $\frac{\Gamma(\sum_{i=1}^k \alpha_i)}{\prod_{i=1}^k \Gamma(\alpha_i)} \prod_{i=1}^k x_i^{\alpha_i - 1}$ | $\frac{\alpha_i}{\sum_{i=1}^k \alpha_i}$ | $\frac{\alpha_i (\sum_{i=1}^k \alpha_i - \alpha_i)}{(\sum_{i=1}^k \alpha_i)^2(\sum_{i=1}^k \alpha_i + 1)}$ | - |
| Beta | $\text{Beta}(\alpha, \beta)$ | $I_x(\alpha, \beta)$ | $\frac{x^{\alpha-1}(1-x)^{\beta-1}}{B(\alpha, \beta)}$ | $\frac{\alpha}{\alpha + \beta}$ | $\frac{\alpha \beta}{(\alpha + \beta)^2(\alpha + \beta + 1)}$ | - |
| Weibull | $\text{Weibull}(\lambda, k)$ | $1 - e^{-(x/\lambda)^k}$ | $\frac{k}{\lambda} \left( \frac{x}{\lambda} \right)^{k-1}e^{-(x/\lambda)^k}$ | $\lambda \Gamma\left(1 + \frac{1}{k}\right)$ | $\lambda^2 \left[ \Gamma\left(1 + \frac{2}{k}\right) - \left(\Gamma\left(1 + \frac{1}{k}\right)\right)^2 \right]$ | - |
| Pareto | $\text{Pareto}(x_m, \alpha)$ | $1 - \left(\frac{x_m}{x}\right)^\alpha \quad x \ge x_m$ | $\frac{\alpha x_m^\alpha}{x^{\alpha + 1}} \quad x \ge x_m$ | $\frac{\alpha x_m}{\alpha - 1} \quad \text{if} \quad \alpha > 1$ | $\frac{\alpha x_m^2}{(\alpha - 1)^2(\alpha - 2)} \quad \text{if} \quad \alpha > 2$ | $\frac{\alpha (-s)^{\alpha}}{\Gamma(-\alpha)}(-s)^{-\alpha} \quad \text{if} \quad s < 0$ |





