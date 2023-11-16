---
aliases: 
publish: true
anki: false
created: 2023-11-15 14:07
parent:
  - "[[Graphical sequence]]"
connected:
  - "[[Havel–Hakimi Theorem]]"
tags:
  - theorem
---

> [!note] Havel–Hakimi Theorem
A sequence ${} s: d_1, d_2, \ldots, d_n$ $(n \geq 2)$ of nonnegative integers with $d_1 \geq d_2 \geq \ldots \geq d_n {}$ is [[Graphical sequence|graphical]]  if and only if ${} \sum_{i=1}^{n} d_i$ is even and for each integer $k$ with $1 \leq k \leq n-1$,
$${} \sum_{i=1}^{k} d_i \leq 2\binom{k}{2} + \sum_{i=k+1}^{n} \min\{k, d_i\} = k(k - 1) + \sum_{i=k+1}^{n} \min\{k, d_i\}.$$



Suppose that $s: d_1, d_2, \ldots, d_n$ is a graphical sequence with $d_1 \geq d_2 \geq \ldots \geq d_n$. Then there exists a graph $G$ of order $n$ with $V(G) = \{v_1, v_2, \ldots, v_n\}$ such that $\deg v_i = d_i$ for all $i (1 \leq i \leq n)$. Of course, the sum $\sum_{i=1}^{n} d_i$ is even. Let $k$ be an integer with $1 \leq k \leq n - 1$. Suppose that $V_1 = \{v_1, v_2, \ldots, v_k\}$ and $V_2 = \{v_{k+1}, v_{k+2}, \ldots, v_n\}$. Now the sum $\sum_{i=1}^{k} d_i$ counts every edge in $G[V_1]$ twice and counts each edge in $[V_1, V_2]$ once. The size of $G[V_1]$ is at most $\binom{k}{2} = k(k - 1)/2$, while for each $i (k + 1 \leq i \leq n)$ the number of edges joining $v_i$ and $V_1$ is at most $\min\{k, d_i\} {}$. Thus,

$${} \sum_{i=1}^{k} d_i \leq 2\binom{k}{2} + \sum_{i=k+1}^{n} \min\{k, d_i\} = k(k - 1) + \sum_{i=k+1}^{n} \min\{k, d_i\}.$$

Hence, for every graphical sequence ${} s$, we must have both that $\sum_{i=1}^{n} d_i$ is even and (1.1) is satisfied for every integer $k$ with $1 \leq k \leq n - 1$. These conditions are not only necessary for a sequence of nonnegative integers to be graphical, but they are sufficient as well. 


