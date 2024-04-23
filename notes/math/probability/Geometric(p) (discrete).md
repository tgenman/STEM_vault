---
aliases: 
publish: true
anki: true
created: 2024-03-20 19:18
parent:
  - "[[Discrete Random Variable]]"
  - "[[Distribution of r.v.]]"
connected: 
tags:
---

> [!tip] Geometric random variable $\text{Geo}(p)$ 
> - [[PMF - p_X(x)|PMF]]: $p_X(x) = p(1-p)^{x-1} \quad x \in \mathbb{N}^+$
> - [[CDF - F_X(x)|CDF]]: $F_X(x) = 1-(1-p)^x \quad x \in \mathbb{N}^+$
> - [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \frac{1}{p}$
> - [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \frac{1-p}{p^2}$
> - [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \frac{pe^s}{1-(1-p)e^s}$  
> - parameter: $0 < p \leq 1$
> - [[Random experiment|Experiment]]: infinitely many independent tosses of a coin; $P(\text{Heads}) = p$
> - [[Sample space]]: Set of infinite sequences of $H$ and $T$
> - Random variable $X$: number of tosses until the first Heads

![[Pasted image 20240423221142.png|400]]
![[Pasted image 20240320191830.png|400]]


$\sum_{k=1}^{\infty} p_X(k) = \sum_{k=1}^{\infty} (1 - p)^{k-1}p = p \sum_{k=0}^{\infty} (1 - p)^k = p \cdot \frac{1}{1 - (1 - p)} = 1$

#### Anki
> [!question]- Geometric discrete r.v.
TARGET DECK: Math::Probability 
START
Math_ONE_side
TITLE: Geometric discrete r.v.
DESCRIPTION: 
> - [[PMF - p_X(x)|PMF]]: $p_X(x) = p(1-p)^{x-1} \quad x \in \mathbb{N}^+$
> - [[CDF - F_X(x)|CDF]]: $F_X(x) = 1-(1-p)^x \quad x \in \mathbb{N}^+$
> - [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \frac{1}{p}$
> - [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \frac{1-p}{p^2}$
> - [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \frac{pe^s}{1-(1-p)e^s}$  
> - parameter: $0 < p \leq 1$
> - [[Random experiment|Experiment]]: infinitely many independent tosses of a coin; $P(\text{Heads}) = p$
> - [[Sample space]]: Set of infinite sequences of $H$ and $T$
> - Random variable $X$: number of tosses until the first Heads
FORMULA: 
ADDITIONAL: $\sum_{k=1}^{\infty} p_X(k) = \sum_{k=1}^{\infty} (1 - p)^{k-1}p = p \sum_{k=0}^{\infty} (1 - p)^k = p \cdot \frac{1}{1 - (1 - p)} = 1$
PICTURE: 
![[Pasted image 20240423221142.png|400]]
![[Pasted image 20240320191830.png|400]]
ID: 1710952073716
END

> [!question]- Expected value of Geometric random variable
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Expected value of Geometric random variable
DESCRIPTION: $\mathbb{E}[X] = \frac{1}{p}$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1713899785152
END

> [!question]- Variance of Geometric random variable
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Variance of Geometric random variable
DESCRIPTION: $\mathbb{V}[X] = \frac{1-p}{p^2}$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1713899785157
END
