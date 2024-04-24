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

### 1.1 Discrete Distributions
- [[Uniform(a, b)  (discrete)]]
- [[Binomial Bin(n, p)]]
	- [[Bernoulli(p)]]  
	- [[Poisson(lambda)]] 
- [[Geometric(p) (discrete)]]

| Distribution      | Notation              | $F_X(x)$                                                  | $f_X(x)$                                              | $\mathbb{E}[X]$        | $\text{Var}[X]$                                                                                                                                                                       | $M_X(s)$                                   |
| ----------------- | --------------------- | --------------------------------------------------------- | ----------------------------------------------------- | ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| Multinomial       | $\text{Mult}(n, p)$   | -                                                         | $\frac{n!}{x_1!\ldots x_k!}p_1^{x_1}\ldots p_k^{x_k}$ | $\sum_{i=1}^k x_i = n$ | $\begin{pmatrix}np_1 & -np_1p_2 & \cdots & -np_1p_k \\ -np_2p_1 & np_2 & \cdots & -np_2p_k \\ \vdots & \vdots & \ddots & \vdots \\ -np_kp_1 & -np_kp_2 & \cdots & np_k \end{pmatrix}$ | $\left( \sum_{i=0}^k p_ie^{s_i} \right)^n$ |
| Hypergeometric    | $\text{Hyp}(N, m, n)$ | $\approx \Phi \left( \frac{x-np}{\sqrt{np(1-p)}} \right)$ | $\frac{\binom{m}{x} \binom{N-m}{n-x}}{\binom{N}{n}}$  | $\frac{nm}{N}$         | $\frac{nm(N-n)(N-m)}{N^2(N-1)}$                                                                                                                                                       | -                                          |
| Negative Binomial | $\text{NB}(r, p)$     | $I_p(r, x+r-1)$                                           | $\binom{x+r-1}{r-1}p^r(1-p)^x$                        | $\frac{r(1-p)}{p}$     | $\frac{r(1-p)}{p^2}$                                                                                                                                                                  | $\left( \frac{p}{1-(1-p)e^s} \right)^r$    |



### 1.2 Continuous Distributions

- [[Uniform(a, b)  (cont)]]
- [[Normal distribution]]
- [[Log-Normal distribution]]
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
- [[Multivariate Normal distribution]]





![[Pasted image 20240423180438.png]]