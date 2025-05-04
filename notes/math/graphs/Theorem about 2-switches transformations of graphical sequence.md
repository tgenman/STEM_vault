---
aliases: 
parent:
  - "[[Graphical sequence]]"
connected:
  - "[[2-switch]]"
  - "[[Theorem about 2-switches transformations of degree sequence]]"
tags:
  - theorem
---

> [!note] Theorem about 2-switches transformations of graphical sequence
Let $s : d_1,d_2,...,d_n$ be a [[Graphical sequence|graphical sequence]] with $∆ = d_1 ≥ d_2 ≥ ··· ≥ d_n$ and let $\mathcal{G}_s$ be the set of all graphs $F$ with [[Degree Sequence|degree sequence]] $s$ such that $V(F)={v_1,v_2,...,v_n}$ where $\deg v_i =d_i$ for $1≤i≤n$. 
Then every graph $H ∈ \mathcal{G}_s$  can be transformed into a graph $G ∈ \mathcal{G}_s$ by a sequence of [[2-switch]]es such that $N_G(v_1) = {v_2, v_3, . . . , v_{∆+1}}$

### Proof. 
Suppose that this statement is false. Let $W=\{v_2,v_3,\ldots,v_{\Delta+1}\}.$ Among all graphs into which $H$ can be transformed, let $G$ be one for which the sum of the subscripts of the vertices in $N_G(v_1)$ is minimum. Since $N_G( v_1) \neq W$, the vertex $v_1$ is adjacent to a vertex $v_k$ and is not adjacent to a vertex $v_j$ with $j<k$ and so $d_j\geq d_k.$ Consequently, there is a vertex $v_{\ell}$ such that $v_jv_{\ell}\in E(G)$ and $v_kv_\ell\not \in E( G) .$ Replacing the edges $v_1v_k$ and $v_jv_\ell$ by $v_1v_j$ and $v_kv_\ell\mathrm{~is~a~2- }$ switch in $G$ that produces a graph $G_1\in\mathcal{G}_s$ for which the sum of the subscripts of the vertices in $N_{G_1}(v_1)$ is less than that of $N_G(v_1).$ Consequently, $H$ can be transformed into $G_1$ and so this is a contradiction.

# Anki
> [!question]-
TARGET DECK: math::graph
START
Math_ONE_side
TITLE: Theorem about 2-switches transformations of graphical sequence
DESCRIPTION: Let $s : d_1,d_2,...,d_n$ be a [[Graphical sequence|graphical sequence]] with $∆ = d_1 ≥ d_2 ≥ ··· ≥ d_n$ and let $\mathcal{G}_s$ be the set of all graphs $F$ with [[Degree Sequence|degree sequence]] $s$ such that $V(F)={v_1,v_2,...,v_n}$ where $\deg v_i =d_i$ for $1≤i≤n$. 
Then every graph $H ∈ \mathcal{G}_s$  can be transformed into a graph $G ∈ \mathcal{G}_s$ by a sequence of [[2-switch]]es such that $N_G(v_1) = {v_2, v_3, . . . , v_{∆+1}}$
FORMULA: 
ADDITIONAL: ### Proof. 
Suppose that this statement is false. Let $W=\{v_2,v_3,\ldots,v_{\Delta+1}\}.$ Among all graphs into which $H$ can be transformed, let $G$ be one for which the sum of the subscripts of the vertices in $N_G(v_1)$ is minimum. Since $N_G( v_1) \neq W$, the vertex $v_1$ is adjacent to a vertex $v_k$ and is not adjacent to a vertex $v_j$ with $j<k$ and so $d_j\geq d_k.$ Consequently, there is a vertex $v_{\ell}$ such that $v_jv_{\ell}\in E(G)$ and $v_kv_\ell\not \in E( G) .$ Replacing the edges $v_1v_k$ and $v_jv_\ell$ by $v_1v_j$ and $v_kv_\ell\mathrm{~is~a~2- }$ switch in $G$ that produces a graph $G_1\in\mathcal{G}_s$ for which the sum of the subscripts of the vertices in $N_{G_1}(v_1)$ is less than that of $N_G(v_1).$ Consequently, $H$ can be transformed into $G_1$ and so this is a contradiction.
ID: 1699170686725
END














