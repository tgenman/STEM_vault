---
aliases: 
publish: true
anki: false
created: 2023-11-24 17:54
parent:
  - "[[Adjacency matrix]]"
  - "[[Walk W]]"
connected: 
tags:
  - theorem
---

> [!note] Theorem about walks in adjacent matrix
Let $G$ be a graph with vertex set $V(G) = \{v_1, v_2, \ldots, v_n\} {}$ and [[Adjacency matrix|adjacency matrix]]  $A$. For each positive integer $k$, the number of different $v_i - v_j {}$  [[Walk W|walks]] of length $k$ in $G$ is the $(i,j)$-entry in the matrix $A^k {}$.

### Proof
Let $a_{ij}^{(k)}$ denote the $(i,j)$-entry in the matrix $A^k$ for a positive integer $k$. Thus, $A^1 = A$ and $a_{ij}^{(1)} = a_{ij}$. We proceed by induction on $k$. For vertices $v_i$ and $v_j$ of $G$, there can be only one $v_i - v_j$ walk of length 1 or no $v_i - v_j$ walks of length 1, and this occurs if $a_{ij} = 1$ or $a_{ij} = 0$, respectively. Therefore, the $(i,j)$-entry of the matrix $A$ is the number of $v_i - v_j$ walks of length 1 in $G$. Thus, the basis step of the induction is established.

We now verify the inductive step. Assume, for a positive integer $k$, that $a_{ij}^{(k)}$ is the number of different $v_i - v_j$ walks of length $k$ in $G$. We show that the $(i,j)$-entry in $A^{k+1}$ gives the number of different $v_i - v_j$ walks of length $k+1$ in $G$. First, observe that every $v_i - v_j$ walk of length $k+1$ in $G$ is obtained from a $v_i - v_t$ walk of length $k$ for some vertex $v_t$ in $G$ that is adjacent to $v_j$.

Since $A^{k+1} = A^k \cdot A$, it follows that the $(i,j)$-entry $a_{ij}^{(k+1)}$ in $A^{k+1}$ can be obtained by taking the inner product of row $i$ of $A^k$ and column $j$ of $A$. That is,

$$
a_{ij}^{(k+1)} = a_{i1}^{(k)}a_{1j} + a_{i2}^{(k)}a_{2j} + \ldots + a_{in}^{(k)}a_{nj} = \sum_{t=1}^{n} a_{it}^{(k)}a_{tj}
$$

By the induction hypothesis, for each integer $t$ with $1 \le t \le n$, the integer $a_{it}^{(k)}$ is the number of different $v_i - v_t$ walks of length $k$ in $G$. If $a_{tj} = 1$, then $v_t$ is adjacent to $v_j$ and so there are $a_{it}^{(k)}$ different $v_i - v_j$ walks of length $k + 1$ in $G$ whose next-to-last vertex is $v_t$. On the other hand, if $a_{tj} = 0$, then $v_t$ is not adjacent to $v_j$ and there are no $v_i - v_j$ walks of length $k + 1$ in $G$ whose next-to-last vertex is $v_t$. In any case, $a_{it}^{(k)} \cdot a_{tj}$ gives the number of different $v_i - v_j$ walks of length $k + 1$ in $G$ whose next-to-last vertex is $v_t$. Consequently, the total number of different $v_i - v_j$ walks of length $k + 1$ in $G$ is the sum in (2.3), which is $a_{ij}^{(k+1)}$.

By the Principle of Mathematical Induction, $a_{ij}^{(k)}$ is the number of different $v_i - v_j$ walks of length $k$ in $G$ for every positive integer $k$. □
















