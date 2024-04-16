---
aliases: 
publish: true
anki: true
created: 2024-03-20 19:18
parent:
  - "[[Discrete Random Variable]]"
connected: 
tags:
---

> [!tip] Geometric random variable
> - parameter: $0 < p \leq 1$
> - [[Random experiment|Experiment]]: infinitely many independent tosses of a coin; $P(\text{Heads}) = p$
> - [[stem/notes/Sample space]]: Set of infinite sequences of $H$ and $T$
> - Random variable $X$: number of tosses until the first Heads

$p_X(k) = (1-p)^{k-1}p, \quad k = 1,2,\dots$

![[Pasted image 20240320191830.png|400]]


$\sum_{k=1}^{\infty} p_X(k) = \sum_{k=1}^{\infty} (1 - p)^{k-1}p = p \sum_{k=0}^{\infty} (1 - p)^k = p \cdot \frac{1}{1 - (1 - p)} = 1$

#### Anki
> [!question]- Geometric discrete r.v.
TARGET DECK: Math::Probability 
START
Math_ONE_side
TITLE: Geometric discrete r.v.
DESCRIPTION: 
> - parameter: $0 < p \leq 1$
> - [[Random experiment|Experiment]]: infinitely many independent tosses of a coin; $P(\text{Heads}) = p$
> - [[stem/notes/Sample space]]: Set of infinite sequences of $H$ and $T$
> - Random variable $X$: number of tosses until the first Heads
FORMULA: $p_X(k) = (1-p)^{k-1}p, \quad k = 1,2,\dots$
ADDITIONAL: $\sum_{k=1}^{\infty} p_X(k) = \sum_{k=1}^{\infty} (1 - p)^{k-1}p = p \sum_{k=0}^{\infty} (1 - p)^k = p \cdot \frac{1}{1 - (1 - p)} = 1$
PICTURE: ![[Pasted image 20240320191830.png]]
ID: 1710952073716
END
