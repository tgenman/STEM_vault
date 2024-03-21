---
aliases: 
publish: true
anki: false
created: 2024-03-21 11:26
parent:
  - "[[Discrete Random Variable]]"
connected:
  - "[[👤 Poisson, Simeon Denis]]"
  - "[[Binomial(n, p) - Binomial r.v.]]"
tags:
  - empty
---

$$ p_X(k) = e^{-\lambda} \frac{\lambda^k}{k!}, \quad k = 0,1,2,\ldots, $$

where $\lambda$ is a positive parameter characterizing the PMF, see Fig. 2.5. This is a legitimate PMF because

$$ \sum_{k=0}^{\infty} e^{-\lambda} \frac{\lambda^k}{k!} = e^{-\lambda} \left(1 + \lambda + \frac{\lambda^2}{2!} + \frac{\lambda^3}{3!} + \ldots\right) = e^{-\lambda}e^{\lambda} = 1. $$

![[Pasted image 20240321113857.png]]

More precisely, the Poisson PMF with parameter $\lambda$ is a good approximation for a [[Binomial(n, p) - Binomial r.v.|binomial]]  PMF with parameters $n$ and $p$, i.e.,

$e^{-\lambda} \frac{\lambda^k}{k!} \approx \frac{n!}{k!(n - k)!} p^k(1 - p)^{n-k}, \quad k = 0,1,\ldots,n$

provided $\lambda = np$, $n$ is very large, and $p$ is very small. In this case, using the Poisson PMF may result in simpler models and calculations. For example, let $n = 100$ and $p = 0.01$. Then the probability of $k = 5$ successes in $n = 100$ trials is calculated using the binomial PMF as

$\frac{100!}{5!95!} 0.01^5(1 - 0.01)^{95} = 0.00290$

Using the Poisson PMF with $\lambda = np = 100 \cdot 0.01 = 1$, this probability is approximated by

$e^{-1} \frac{1^5}{5!} = 0.00306$


