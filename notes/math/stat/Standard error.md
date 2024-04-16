---
aliases: 
publish: true
anki: false
created: 2024-04-11 15:39
parent:
  - "[[Variance V(X)]]"
connected:
  - "[[Standard deviation]]"
tags:
  - empty
---

> [!tip] Standard error
describes [[Random noise|noisiness]]  of an [[Point estimate|estimate]]:
$\text{se}(\hat{\theta}) = \sqrt{\text{Var}\hat{\theta}}$

**Example.**
Let $X_1, \ldots, X_n \sim \text{Bernoulli}(p)$ and let $\hat{p}_n = n^{-1} \sum_i X_i$. Then $\mathbb{E}(\hat{p}_n) = p$ so $\hat{p}_n$ is unbiased. The standard error is $\text{se} = \sqrt{p(1 - p)/n}$. The estimated standard error is $\hat{\text{se}} = \sqrt{\hat{p}(1 - \hat{p})/n}$.