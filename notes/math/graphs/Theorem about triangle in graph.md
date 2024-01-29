---
aliases: 
tags:
  - theorem
publish: true
anki: true
created: 2023-11-03 16:57
parent:
  - "[[519.17 Graph Theory MOC]]"
connected:
  - "[[Triangle (graph)]]"
---
> [!note] Theorem about triangle in graph
Every [[Simple Graph (G)|graph]] of order $n ≥ 3$ and size $m > ⌊\frac{n^2}{4}⌋$ contains a [[Triangle (graph)|triangle]].

### Proof
First, observe that the result is true for $n= 3$ and $n= 4.$ Suppose, however, that the statement is false. Then there is a smallest integer $n\geq 5$ and a graph $G$ of order $n$ and size $m>|n^2/4]$ not containing a trianglc. Let $uv$ be an edge of $G.$ Since $G$ contains no triangle, there is no vertex in $G$ adjacent to both $u$ and $v.$ Hence, $(\deg u-1)+(\deg v-1)\leq n-2$ and so $\deg u+\deg v\leq n.$ Let $G^{\prime}= G- u- v.$ Since $G^{\prime}$ is a subgraph of $G, $it follows that $G^{\prime}$ also does not contain a triangle. Furthermore, $G^{\prime}$ has order $n- 2$ and size

$$m^{\prime}=m-(\deg u+\deg v)+1>\lfloor n^2/4\rfloor-n+1.$$

Thus,
$$m^{\prime}>\frac{n^2}4-n+1=\frac{n^2-4n+4}4=\frac{(n-2)^2}4.$$

From the defining property of the graph $G$, it follows that $G^{\prime}$ contains a triangle producing a contradiction.

### Anki
> [!question]-
TARGET DECK: Math::Graph
START
Math prop
TITLE: Theorem about triangle in graph
TITLE_rus: 
DESCRIPTION: Every [[Simple Graph (G)|graph]] of order $n ≥ 3$ and size $m > ⌊\frac{n^2}{4}⌋$ contains a [[Triangle (graph)|triangle]].
DESCRIPTION_rus: 
Formula_main: 
Formula_additional: ### Proof
First, observe that the result is true for $n= 3$ and $n= 4.$ Suppose, however, that the statement is false. Then there is a smallest integer $n\geq 5$ and a graph $G$ of order $n$ and size $m>|n^2/4]$ not containing a trianglc. Let $uv$ be an edge of $G.$ Since $G$ contains no triangle, there is no vertex in $G$ adjacent to both $u$ and $v.$ Hence, $(\deg u-1)+(\deg v-1)\leq n-2$ and so $\deg u+\deg v\leq n.$ Let $G^{\prime}= G- u- v.$ Since $G^{\prime}$ is a subgraph of $G, $it follows that $G^{\prime}$ also does not contain a triangle. Furthermore, $G^{\prime}$ has order $n- 2$ and size
$$m^{\prime}=m-(\deg u+\deg v)+1>\lfloor n^2/4\rfloor-n+1.$$
Thus,
$$m^{\prime}>\frac{n^2}4-n+1=\frac{n^2-4n+4}4=\frac{(n-2)^2}4.$$
From the defining property of the graph $G$, it follows that $G^{\prime}$ contains a triangle producing a contradiction.
<!--ID: 1699170839925-->
END












