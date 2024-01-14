---
aliases:
  - Порожденный подграф
publish: true
anki: false
created: 2023-11-01 15:28
parent:
  - "[[Subgraph]]"
connected:
---

> [!tip] Induced subgraph
is a subgraph $H$ of $G {}$ if: 
> - there is a nonempty vertex subset $S$ of $V(G)$ such that $H = G[S]$.

$G[V(G)] = G {}$. 

> [!tip] Edge-induced subgraph
> is a subgraph $H$ of $G {}$ if:
> - there is a nonempty  edge subset $X$ of $E(G)$ such that $H = G[X] {}$. 

Thus, $G[E(G)] = G$ if and only if $G {}$ has no isolated vertices.

If  $E(H) = E(G) \cap \binom{V(H)}{2} {}$ then $H {}$ is induced subgraph
### Induced by
> [!tip] Induced by vertex set $S {}$
> Subgraph $G[S]$ of $G$ induced by $S {}$ (for a nonempty  vertex subset $S$ of $V(G) {}$) if:
> - has $S$ as its vertex set and
> - two vertices $u$ and $v$ are adjacent in $G[S]$ if and only if $u$ and $v$ are adjacent in $G {}$.

> [!tip] Induced by edge set $X {}$
> Subgraph $G[X] {}$ of $G$ induced by $X {}$ (for a nonempty  edge subset $X$ of $E{} (G) {}$) if:
> - has $X {}$ as its edge set and
> - a vertex $v$ belongs to $G[X]$ if $v$ is incident with at least one edge in $X$. 

### Anki
> [!question]-
TARGET DECK: Math::Graph
START
Math prop
Question_eng: Induced subgraph
Question_rus: 
Answer_eng: is a subgraph $H$ of $G {}$ if: 
if there is a nonempty vertex subset $S$ of $V(G)$ such that $H = G[S]$.
$G[V(G)] = G {}$. 
Answer_rus: 
Formula_main: 
Formula_additional:
<!--ID: 1699171145822-->
END

> [!question]-
TARGET DECK: Math::Graph
START
Math prop
Question_eng: Edge-induced subgraph
Question_rus: 
Answer_eng: is a subgraph $H$ of $G {}$ if:
there is a nonempty  edge subset $X$ of $E(G)$ such that $H = G[X]$. 
Thus, $G[E(G)] = G$ if and only if $G {}$ has no isolated vertices.
Answer_rus: 
Formula_main: 
Formula_additional:
<!--ID: 1699171145833-->
END

> [!question]-
TARGET DECK: Math::Graph
START
Math prop
Question_eng: Induced by vertex set $S {}$
Question_rus: 
Answer_eng: Subgraph $G[S]$ of $G$ induced by $S {}$ (for a nonempty  vertex subset $S$ of $V(G) {}$) if:
 has $S$ as its vertex set and
 two vertices $u$ and $v$ are adjacent in $G[S]$ if and only if $u$ and $v$ are adjacent in $G {}$.
Answer_rus: 
Formula_main: 
Formula_additional:
<!--ID: 1699171145843-->
END

> [!question]-
TARGET DECK: Math::Graph
START
Math prop
Question_eng: Induced by edge set $X {}$
Question_rus: 
Answer_eng: > Subgraph $G[X] {}$ of $G$ induced by $X {}$ (for a nonempty  edge subset $X$ of $E{} (G) {}$) if:
 has $X {}$ as its edge set and
 a vertex $v$ belongs to $G[X]$ if $v$ is incident with at least one edge in $X$. 
Answer_rus: 
Formula_main: 
Formula_additional:
<!--ID: 1699171145854-->
END










