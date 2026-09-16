---
aliases: 
anki: false
created: 2024-04-24 17:13
parent:
  - "[[Discrete Random Variable]]"
  - "[[Distribution of r.v. MOC]]"
connected:
  - "[[Binomial distribution Bin(n, p)]]"
tags:
---

> [!tip] Hypergeometric $\operatorname{Hyp}(N,m,n)$
> The number $X$ of marked objects in a uniformly selected sample of $n$ objects drawn without replacement from $N$ objects, of which $m$ are marked.

Assume integers $N\ge1$, $0\le m\le N$, $0\le n\le N$. Set $L=\max(0,n-(N-m))$ and $U=\min(n,m)$.

- [[PMF - p_X(x)|PMF]]: $P(X=k)=\binom{m}{k}\binom{N-m}{n-k}/\binom{N}{n}$ for integers $L\le k\le U$, and zero otherwise.
- [[CDF - F_X(x)|CDF]]: $F_X(x)=\sum_{k=L}^{\min(U,\lfloor x\rfloor)}P(X=k)$, with an empty sum equal to zero.
- [[Expected Value E(X)|Mean]]: $nm/N$.
- [[Variance V(X)|Variance]] for $N>1$: $\frac{nm(N-n)(N-m)}{N^2(N-1)}$. The $N=1$ cases are deterministic.
- [[Производящая функция моментов случайной M_X(s)|MGF]]: $M_X(s)=\sum_{k=L}^{U}e^{sk}P(X=k)$.

Source: [R stats: hypergeometric](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/Hypergeometric.html). R uses numbers of marked/unmarked objects and draws; here the notation is $(N,m,n)$.
