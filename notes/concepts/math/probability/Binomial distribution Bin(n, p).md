---
aliases: 
anki: true
created: 2024-03-20 19:02
parent:
  - "[[Bernoulli(p)]]"
  - "[[Discrete Random Variable]]"
  - "[[Distribution of r.v. MOC]]"
connected:
  - "[[Схема испытиний Бернулли]]"
  - "[[Poisson(lambda)]]"
  - "[[Multinomial formula]]"
  - "[[Negative Binomial NB(r, p)]]"
tags:
---

> [!tip] Binomial r.v.  $\text{Bin}(n, p)$
- [[PMF - p_X(x)|PMF]]: $p_X(x) = \binom{n}{x}p^x(1-p)^{n-x}$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = \sum_{k=0}^{\min(n,\lfloor x\rfloor)}\binom nk p^k(1-p)^{n-k}\quad(x\ge0);\quad F_X(x)=0\ (x<0)$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = np$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = np(1-p)$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = (1-p+pe^s)^n$  
- is multiple [[Bernoulli(p)]]:
- [[Random experiment|experiment]]: $n$ independent tosses of a coin with $P(\text{Heads}) = p$
- [[Sample space]]: Set of sequences of $H$ and $T$, of length $n$
- Random variable $X$: number of Heads observed
- Model of: number of successes in a given number of independent trials

$\sum_{k=0}^{n} \binom{n}{k} p^k (1-p)^{n-k} = 1$

![[Pasted image 20240423220214.png|400]]

![[Pasted image 20240320191223.png|300]]

![[Pasted image 20240320191248.png]]

## связи распределений

For mutually independent variables with common success probability $p$:
- $X_i\sim\operatorname{Bern}(p)\ \Rightarrow\ \sum_{i=1}^nX_i\sim\operatorname{Bin}(n,p)$.
- $X\sim\operatorname{Bin}(n,p)$, $Y\sim\operatorname{Bin}(m,p)\ \Rightarrow\ X+Y\sim\operatorname{Bin}(n+m,p)$.

For $X_n\sim\operatorname{Bin}(n,p_n)$, if $n\to\infty$, $p_n\to0$ and $np_n\to\lambda>0$, then $X_n\xrightarrow{d}\operatorname{Po}(\lambda)$.

For fixed $p\in(0,1)$,
$$
\frac{X_n-np}{\sqrt{np(1-p)}}\xrightarrow{d}\mathcal N(0,1).
$$
The unstandardized normal approximation uses mean $np$ and variance $np(1-p)$; it is not an equality of limiting distributions with changing parameters.

Sources: [sums of independent variables](https://heogden.github.io/math2011/sums-of-random-variables.html), [binomial distribution](https://www.statlect.com/probability-distributions/binomial-distribution), [Poisson limit](https://www.statlect.com/probability-distributions/Poisson-distribution).

# Anki
TARGET DECK: math::probability
START
math_complex
FRONT: Binomial r.v.  $\text{Bin}(n, p)$
BACK: 
- [[PMF - p_X(x)|PMF]]: $p_X(x) = \binom{n}{x}p^x(1-p)^{n-x}$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = \sum_{k=0}^{\min(n,\lfloor x\rfloor)}\binom nk p^k(1-p)^{n-k}\quad(x\ge0);\quad F_X(x)=0\ (x<0)$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = np$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = np(1-p)$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = (1-p+pe^s)^n$  
- is multiple [[Bernoulli(p)]]:
- [[Random experiment|experiment]]: $n$ independent tosses of a coin with $P(\text{Heads}) = p$
- [[Sample space]]: Set of sequences of $H$ and $T$, of length $n$
- Random variable $X$: number of Heads observed
- Model of: number of successes in a given number of independent trials
FORMULA: 
$\sum_{k=0}^{n} \binom{n}{k} p^k (1-p)^{n-k} = 1$
ADDITIONAL:
PICTURE:
![[Pasted image 20240423220214.png|400]]
![[Pasted image 20240320191223.png|300]]
![[Pasted image 20240320191248.png]]
ID: 1710951460558
END

TARGET DECK: math::probability
START
math_complex
FRONT: Expected value of Binomial Distribution
BACK: $\mathbb{E}[X] = np$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1713899360759
END

TARGET DECK: math::probability
START
math_complex
FRONT: Variance of Binomial Distribution
BACK: $\mathbb{V}[X] = np(1-p)$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1713899360764
END
