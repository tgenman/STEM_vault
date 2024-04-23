---
aliases: 
publish: true
anki: true
created: 2024-03-20 19:02
parent:
  - "[[Bernoulli(p)]]"
  - "[[Discrete Random Variable]]"
  - "[[Distribution of r.v.]]"
connected:
  - "[[Схема испытиний Бернулли]]"
tags:
---

> [!tip] Binomial r.v.  $\text{Bin}(n, p)$
> - [[PMF - p_X(x)|PMF]]: $p_X(x) = \binom{n}{x}p^x(1-p)^{n-x}$
> - [[CDF - F_X(x)|CDF]]: $F_X(x) = I_{1-p}(n-x, x+1)$
> - [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = np$
> - [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = np(1-p)$
> - [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = (1-p+pe^s)^n$  
> - is multiple [[Bernoulli(p)]]:
> - [[Random experiment|experiment]]: $n$ independent tosses of a coin with $P(\text{Heads}) = p$
> - [[Sample space]]: Set of sequences of $H$ and $T$, of length $n$
> - Random variable $X$: number of Heads observed
> - Model of: number of successes in a given number of independent trials

$\sum_{k=0}^{n} \binom{n}{k} p^k (1-p)^{n-k} = 1$

![[Pasted image 20240423220214.png|400]]

![[Pasted image 20240320191223.png|300]]

![[Pasted image 20240320191248.png]]

#### Anki
> [!question]- Binomial r.v.  $\text{Bin}(n, p)$
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Binomial r.v.  $\text{Bin}(n, p)$
DESCRIPTION: 
> - [[PMF - p_X(x)|PMF]]: $p_X(x) = \binom{n}{x}p^x(1-p)^{n-x}$
> - [[CDF - F_X(x)|CDF]]: $F_X(x) = I_{1-p}(n-x, x+1)$
> - [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = np$
> - [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = np(1-p)$
> - [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = (1-p+pe^s)^n$  
> - is multiple [[Bernoulli(p)]]:
> - [[Random experiment|experiment]]: $n$ independent tosses of a coin with $P(\text{Heads}) = p$
> - [[Sample space]]: Set of sequences of $H$ and $T$, of length $n$
> - Random variable $X$: number of Heads observed
> - Model of: number of successes in a given number of independent trials
FORMULA: 
$\sum_{k=0}^{n} \binom{n}{k} p^k (1-p)^{n-k} = 1$
ADDITIONAL:
PICTURE:
![[Pasted image 20240423220214.png|400]]
![[Pasted image 20240320191223.png|300]]
![[Pasted image 20240320191248.png]]
ID: 1710951460558
END

> [!question]- Expected value of Binomial Distribution
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Expected value of Binomial Distribution
DESCRIPTION: $\mathbb{E}[X] = np$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1713899360759
END

> [!question]- Variance of Binomial Distribution
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Variance of Binomial Distribution
DESCRIPTION: $\mathbb{V}[X] = np(1-p)$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1713899360764
END