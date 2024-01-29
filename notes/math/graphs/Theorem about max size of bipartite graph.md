---
aliases: 
tags:
  - theorem
publish: true
anki: true
created: 2023-11-03 16:35
parent:
  - "[[519.172.5 Bipartite graph]]"
connected:
  - "[[Size of graph (m)]]"
---

> [!note] Theorem about max size of bipartite graph
The [[Size of graph (m)|size]] of every ==bipartite graph== of order $n$ is at most $⌊\frac{n^2}{4}⌋$

### Proof
Let $G$ be bipartite graph of order $n$ with partite sets $U$ and $W.$ Then $|U|= x$ and $|W|= n- x$ for some integer $x$ with $1\leq x\leq n- 1.$ Hence the size of $G$ is at most $x(n-x).$

Since $(n-2x)^2\geq0$, it follows that
$$n^2\geq4nx-4x^2=4x(n-x)$$
and so $x(n-x)\leq n^2/4.$ Since $x(n-x)$ is an integer, $x(n-x)\leq\lfloor n^2/4\rfloor.$


### Anki
> [!question]-
TARGET DECK: Math::Graph
START
Math prop
TITLE: Theorem about max size of bipartite graph
TITLE_rus: 
Answer_eng: The [[Size of graph (m)|size]] of every ==bipartite graph== of order $n$ is at most $⌊\frac{n^2}{4}⌋$
Answer_rus: 
Formula_main: 
Formula_additional: ### Proof
Let $G$ be bipartite graph of order $n$ with partite sets $U$ and $W.$ Then $|U|= x$ and $|W|= n- x$ for some integer $x$ with $1\leq x\leq n- 1.$ Hence the size of $G$ is at most $x(n-x).$
Since $(n-2x)^2\geq0$, it follows that
$$n^2\geq4nx-4x^2=4x(n-x)$$
and so $x(n-x)\leq n^2/4.$ Since $x(n-x)$ is an integer, $x(n-x)\leq\lfloor n^2/4\rfloor.$
<!--ID: 1699170792069-->
END












