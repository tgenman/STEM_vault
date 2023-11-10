---
aliases:
  - Двупольный граф
publish: true
anki: true
created: 2023-11-03 16:20
parent:
  - "[[Graph (G)]]"
connected:
  - "[[Bipartite graph]]"
  - "[[Complete bipartite graph]]"
---

> [!tip] A graph ${} G$ is bipartite 
if ${} V(G)$ can be partitioned into two sets $U$ and $W {}$ (called partite sets) so that every  [[Edge of graph (E)|edge]] of ${} G {}$ joins a [[Vertex of graph (V)|vertex]]  of ${} U$ and a vertex of $W {}$

![[Pasted image 20231103162131.png]]
typical bipartite graphs:
- [[Path graph (P_n)]]
- even order [[Cycle graph (C_n)]]


Therefore, from [[Theorem about max size of bipartite graph]] and [[Theorem about triangle in graph]], it follows that every graph of order ${} n ≥ 3$ and size ${} m > ⌊\frac{n^2}{4}⌋$ not only fails to be ==bipartite==, it must, in fact, contain a [[Triangle]].

[[Complete bipartite graph]]
[[Multipartite Graphs]]
[[Complete multipartite Graphs]]


### Anki
> [!question]-
START
Math prop
Question_eng: A graph ${} G$ is bipartite 
Question_rus: 
Answer_eng: if ${} V(G)$ can be partitioned into two sets $U$ and $W {}$ (called partite sets) so that every  [[Edge of graph (E)|edge]] of ${} G {}$ joins a [[Vertex of graph (V)|vertex]]  of ${} U$ and a vertex of $W {}$
Answer_rus: 
Formula_main: ![[Pasted image 20231103162131.png]]
Formula_additional: Therefore, from [[Theorem about max size of bipartite graph]] and [[Theorem about triangle in graph]], it follows that every graph of order ${} n ≥ 3$ and size ${} m > ⌊\frac{n^2}{4}⌋$ not only fails to be ==bipartite==, it must, in fact, contain a [[Triangle]].
<!--ID: 1699126412967-->
END