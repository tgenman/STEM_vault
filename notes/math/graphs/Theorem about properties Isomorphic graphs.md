---
aliases: 
tags:
  - theorem
parent: 
connected:
  - "#обс/linking"
---

> [!note] Theorem Properties Isomorphic graphs
If two graphs $G$ and $H$ are [[519.175.1 Isomorphic Graphs|isomorphic]], then they have the same [[Order of graph (n)|order]] and the same [[Size of graph (m)|size]], and the [[Degree of a vertex (deg)|degrees]] of the vertices of $G$ are the same as the degrees of the vertices of $H$
$|V (G)| = |V (H)|$
$|E(G)| = |E(H)|$

### Proof
We have already observed that isomorphic graphs have the same order and the same size. Let $v$ be a vertex of $G$ and suppose that $\deg v=k.$ Then $v$ is adjacent to $k$ vertices, say $v_1,v_2,\ldots,v_k.$ Suppose that $v$ is not adjacent to $u_1,u_2,\ldots,u_\ell.$ If $\phi:V(G)\to V(H)$ is an isomorphism, then $\phi(v)$ is adjacent to $\phi(v_1),\phi(v_2),\ldots,\phi(v_k)$ while $\phi(v)$ is not adjacent to $\phi(u_1),\phi(u_2),\ldots,\phi(u_\ell).$ Hence, $\phi(v)$ has degree $k$ in $H.$

# Anki
TARGET DECK: math::graph
START
math_complex
FRONT: Theorem about properties Isomorphic graphs
BACK: If two graphs $G$ and $H$ are [[519.175.1 Isomorphic Graphs|isomorphic]], then they have the same [[Order of graph (n)|order]] and the same [[Size of graph (m)|size]], and the [[Degree of a vertex (deg)|degrees]] of the vertices of $G$ are the same as the degrees of the vertices of $H$
$|V (G)| = |V (H)|$
$|E(G)| = |E(H)|$
FORMULA: 
ADDITIONAL: ### Proof
We have already observed that isomorphic graphs have the same order and the same size. Let $v$ be a vertex of $G$ and suppose that $\deg v=k.$ Then $v$ is adjacent to $k$ vertices, say $v_1,v_2,\ldots,v_k.$ Suppose that $v$ is not adjacent to $u_1,u_2,\ldots,u_\ell.$ If $\phi:V(G)\to V(H)$ is an isomorphism, then $\phi(v)$ is adjacent to $\phi(v_1),\phi(v_2),\ldots,\phi(v_k)$ while $\phi(v)$ is not adjacent to $\phi(u_1),\phi(u_2),\ldots,\phi(u_\ell).$ Hence, $\phi(v)$ has degree $k$ in $H.$
ID: 1699129856552
END












