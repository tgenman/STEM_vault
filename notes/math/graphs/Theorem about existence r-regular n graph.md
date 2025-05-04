---
aliases: 
created: 2023-11-04 17:57
parent:
  - "[[519.172.4 Regular Graphs]]"
connected: 
tags:
  - theorem
---

> [!note] Theorem
> For integers $r$ and $n$, there exists an $r$-regular graph of order $n$ if and only if
> - $0 ≤ r ≤ n − 1$ 
> - $r$ and $n$ are not both odd.

### Proof
That the conditions are necessary is an immediate consequence of Corollary 1.5 and the fact that $0\leq\deg v\leq n-1$ for every vertex $v$ in a graph of order $n.$ For the converse, suppose that $r$ and $n$ are integers where $0\leq r\leq n- 1$ and $r$ and $n$ are not both odd. Assume first that $r$ is even. If $r= 0$, then the graph of order $n$ consisting of $n$ isolated vertices is $r$-regular. So we may assume that $r=2k$ for some integer $k\geq 1$ and $n\geq 2k+ 1.$ Let $G$ be the graph with $V(G)=\{v_1,v_2,\ldots,v_n\}$ such that $v_i\left(1\leq i\leq n\right)$ is adjacent to $v_{i\pm1},v_{i\pm2},\ldots,v_{i\pm k}$ (subscripts expressed modulo $n$ . The resulting graph $G$ is then an $r$-regular graph of order $n$. If $r$ is odd, then $n=2\ell$ is even. Hence $r=2k+1$ for some integer $k$ with $0\leq k\leq\ell-1.$ For the graph $G$ in this case, the vertex $v_i$ is adjacent to the $2k$ vertices described above and adjacent as well to $v_{i+\ell}$. Again, $G$ is an $r$-regular graph of order $n.$

 ![[Pasted image 20231101184533.png]]

### Anki
> [!question]-
TARGET DECK: math::graph
START
Math_ONE_side
TITLE: Theorem about existence r-regular n graph
DESCRIPTION: For integers $r$ and $n$, there exists an $r$-regular graph of order $n$ if and only if
$0 ≤ r ≤ n − 1$ 
$r$ and $n$ are not both odd.
FORMULA: 
ADDITIONAL: That the conditions are necessary is an immediate consequence of Corollary 1.5 and the fact that $0\leq\deg v\leq n-1$ for every vertex $v$ in a graph of order $n.$ For the converse, suppose that $r$ and $n$ are integers where $0\leq r\leq n- 1$ and $r$ and $n$ are not both odd. Assume first that $r$ is even. If $r= 0$, then the graph of order $n$ consisting of $n$ isolated vertices is $r$-regular. So we may assume that $r=2k$ for some integer $k\geq 1$ and $n\geq 2k+ 1.$ Let $G$ be the graph with $V(G)=\{v_1,v_2,\ldots,v_n\}$ such that $v_i\left(1\leq i\leq n\right)$ is adjacent to $v_{i\pm1},v_{i\pm2},\ldots,v_{i\pm k}$ (subscripts expressed modulo $n$ . The resulting graph $G$ is then an $r$-regular graph of order $n$. If $r$ is odd, then $n=2\ell$ is even. Hence $r=2k+1$ for some integer $k$ with $0\leq k\leq\ell-1.$ For the graph $G$ in this case, the vertex $v_i$ is adjacent to the $2k$ vertices described above and adjacent as well to $v_{i+\ell}$. Again, $G$ is an $r$-regular graph of order $n.$
 ![[Pasted image 20231101184533.png]]
ID: 1699170748365
END
















