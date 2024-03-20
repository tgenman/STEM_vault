---
aliases: 
publish: true
anki: true
created: 2024-03-20 19:02
parent:
  - "[[Bernoulli r.v.]]"
connected: 
tags:
  - empty
---

> [!tip] Binomial r.v. parameter n
> is multiple [[Bernoulli r.v.]]:
> - [[Random experiment|experiment]]: $n$ independent tosses of a coin with $P(\text{Heads}) = p$
> - [[Sample space]]: Set of sequences of $H$ and $T$, of length $n$
> - Random variable $X$: number of Heads observed
> - Model of: number of successes in a given number of independent trials

$p_X(k) = P(X = k) = \binom{n}{k} p^k (1-p)^{n-k}; \quad k = 0,1,\dots,n.$

$\sum_{k=0}^{n} \binom{n}{k} p^k (1-p)^{n-k} = 1$


![[Pasted image 20240320191223.png|300]]


![[Pasted image 20240320191248.png]]

#### Anki
> [!question]- Binomial r.v. Bin(n)
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Binomial r.v. Bin(n)
DESCRIPTION: 
> is multiple [[Bernoulli r.v.]]:
> - [[Random experiment|experiment]]: $n$ independent tosses of a coin with $P(\text{Heads}) = p$
> - [[Sample space]]: Set of sequences of $H$ and $T$, of length $n$
> - Random variable $X$: number of Heads observed
> - Model of: number of successes in a given number of independent trials
FORMULA: 
$p_X(k) = P(X = k) = \binom{n}{k} p^k (1-p)^{n-k}; \quad k = 0,1,\dots,n.$
$\sum_{k=0}^{n} \binom{n}{k} p^k (1-p)^{n-k} = 1$
ADDITIONAL:
PICTURE:
![[Pasted image 20240320191223.png|300]]
![[Pasted image 20240320191248.png]]
ID: 1710951460558
END