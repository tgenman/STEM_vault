---
aliases: 
created: 2023-11-01 12:07
parent:
  - "[[Vertex of graph (V)]]"
connected:
  - "#обс/linking"
tags:
  - corollary
---
> [!info] Corollary
> Every graph has an even number of odd vertices.

### Proof
Proof. Suppose that $G$ is a graph of size $m$. By [[Handshaking Lemma]],
$$\sum_{v\in V(G)}\deg v=2m.$$
which, of course, is an even number. Since the sum of the degrees of the even vertices of $G$ is even, the sum of the degrees of the odd vertices of $G$ must be even as well, implying that $G$ has an even number of odd vertices.

 # Anki
TARGET DECK: math::graph
START
math_complex
FRONT: Number of odd vertices (corollary)
BACK: Every graph has an even number of odd vertices.
FORMULA: 
ADDITIONAL: ### Proof
Proof. Suppose that $G$ is a graph of size $m$. By [[Handshaking Lemma]],
$$\sum_{v\in V(G)}\deg v=2m.$$
which, of course, is an even number. Since the sum of the degrees of the even vertices of $G$ is even, the sum of the degrees of the odd vertices of $G$ must be even as well, implying that $G$ has an even number of odd vertices.
ID: 1699164385575
END












