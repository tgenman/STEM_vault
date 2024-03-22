---
aliases: 
publish: true
anki: true
created: 2024-03-21 11:26
parent:
  - "[[Discrete Random Variable]]"
connected:
  - "[[👤 Poisson, Simeon Denis]]"
  - "[[Binomial(n, p)]]"
tags:
---

> [!tip] Poisson($\lambda$)
$p_X(k) = e^{-\lambda} \frac{\lambda^k}{k!}, \quad k = 0,1,2,\ldots$

where $\lambda$ is a positive parameter characterizing the PMF, see Fig. 2.5. 

This is a legitimate PMF because
$\sum_{k=0}^{\infty} e^{-\lambda} \frac{\lambda^k}{k!} = e^{-\lambda} \left(1 + \lambda + \frac{\lambda^2}{2!} + \frac{\lambda^3}{3!} + \ldots\right) = e^{-\lambda}e^{\lambda} = 1$

![[Pasted image 20240321113857.png]]

More precisely, the Poisson PMF with parameter $\lambda$ is a good approximation for a [[Binomial(n, p)|binomial]]  PMF with parameters $n$ and $p$, i.e.,

$e^{-\lambda} \frac{\lambda^k}{k!} \approx \frac{n!}{k!(n - k)!} p^k(1 - p)^{n-k}, \quad k = 0,1,\ldots,n$

provided $\lambda = np$, $n$ is very large, and $p$ is very small. In this case, using the Poisson PMF may result in simpler models and calculations. For example, let $n = 100$ and $p = 0.01$. Then the probability of $k = 5$ successes in $n = 100$ trials is calculated using the binomial PMF as

$\frac{100!}{5!95!} 0.01^5(1 - 0.01)^{95} = 0.00290$

Using the Poisson PMF with $\lambda = np = 100 \cdot 0.01 = 1$, this probability is approximated by

$e^{-1} \frac{1^5}{5!} = 0.00306$


#### [[Expected Value E(X)]]
$E[X] = \lambda$

###### Proof
$E[X] = \sum_{k=0}^{\infty} ke^{-\lambda} \frac{\lambda^k}{k!}$

Since the term for $k=0$ is zero (as it results in $0$ multiplied by some constant), we start from $k=1$:
$E[X] = \sum_{k=1}^{\infty} ke^{-\lambda} \frac{\lambda^k}{k!}= \lambda \sum_{k=1}^{\infty} e^{-\lambda} \frac{\lambda^{k-1}}{(k-1)!}$

Let $m = k - 1$, then the sum turns into:
$E[X]= \lambda \sum_{m=0}^{\infty} e^{-\lambda} \frac{\lambda^m}{m!}$

Since$\sum_{m=0}^{\infty} e^{-\lambda} \frac{\lambda^m}{m!} = \sum_{m=0}^{\infty} p_X(m) = 1$:
$E[X] = \lambda$

#### [[Variance V(X)]]
$V[X] = \lambda$


#### Anki
> [!question]- Poisson($\lambda$)
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Poisson($\lambda$)
DESCRIPTION: $p_X(k) = e^{-\lambda} \frac{\lambda^k}{k!}, \quad k = 0,1,2,\ldots$
where $\lambda$ is a positive parameter characterizing the PMF, see Fig. 2.5. 
FORMULA: This is a legitimate PMF because
$\sum_{k=0}^{\infty} e^{-\lambda} \frac{\lambda^k}{k!} = e^{-\lambda} \left(1 + \lambda + \frac{\lambda^2}{2!} + \frac{\lambda^3}{3!} + \ldots\right) = e^{-\lambda}e^{\lambda} = 1$
ADDITIONAL: More precisely, the Poisson PMF with parameter $\lambda$ is a good approximation for a [[Binomial(n, p)|binomial]]  PMF with parameters $n$ and $p$, i.e.,
$e^{-\lambda} \frac{\lambda^k}{k!} \approx \frac{n!}{k!(n - k)!} p^k(1 - p)^{n-k}, \quad k = 0,1,\ldots,n$
provided $\lambda = np$, $n$ is very large, and $p$ is very small. In this case, using the Poisson PMF may result in simpler models and calculations. For example, let $n = 100$ and $p = 0.01$. Then the probability of $k = 5$ successes in $n = 100$ trials is calculated using the binomial PMF as
$\frac{100!}{5!95!} 0.01^5(1 - 0.01)^{95} = 0.00290$
Using the Poisson PMF with $\lambda = np = 100 \cdot 0.01 = 1$, this probability is approximated by
$e^{-1} \frac{1^5}{5!} = 0.00306$
PICTURE: ![[Pasted image 20240321113857.png]]
ID: 1711025905236
END

> [!question]- Expected Value E(X) of Poisson($\lambda$)
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Expected Value E(X) of Poisson($\lambda$)
DESCRIPTION: $E[X] = \lambda$
FORMULA: 
ADDITIONAL: Proof
$E[X] = \sum_{k=0}^{\infty} ke^{-\lambda} \frac{\lambda^k}{k!}$
Since the term for $k=0$ is zero (as it results in $0$ multiplied by some constant), we start from $k=1$:
$E[X] = \sum_{k=1}^{\infty} ke^{-\lambda} \frac{\lambda^k}{k!}= \lambda \sum_{k=1}^{\infty} e^{-\lambda} \frac{\lambda^{k-1}}{(k-1)!}$
Let $m = k - 1$, then the sum turns into:
$E[X]= \lambda \sum_{m=0}^{\infty} e^{-\lambda} \frac{\lambda^m}{m!}$
Since$\sum_{m=0}^{\infty} e^{-\lambda} \frac{\lambda^m}{m!} = \sum_{m=0}^{\infty} p_X(m) = 1$:
$E[X] = \lambda$
PICTURE:
ID: 1711025905248
END

> [!question]- Variance V(X) of Poisson($\lambda$)
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Variance V(X) of Poisson($\lambda$)
DESCRIPTION: $V[X] = \lambda$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1711025905251
END