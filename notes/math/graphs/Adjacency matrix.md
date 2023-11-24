---
aliases:
  - Матрица смежности
publish: true
anki: false
created: 2023-11-23 22:00
parent:
  - "[[Simple Graph (G)|Graph]]"
connected:
  - "[[Matrix]]"
---

> [!tip] The adjacency matrix
 Suppose that ${} G$ is a graph of order $n$, where $V(G) = \{v_1, v_2, \ldots, v_n\}$. The adjacency matrix of $G$ is the $n \times n$ zero-one matrix $A(G) = [a_{ij}]$, or simply $A = [a_{ij}]$, where

$$
a_{ij} = 
\begin{cases} 
1 & \text{if } v_iv_j \in E(G) \\
0 & \text{if } v_iv_j \not\in E(G).
\end{cases}
$$
![[Pasted image 20231123220529.png]]

- all entries along the main diagonal of $A {}$ are $0 {}$ since no vertex of $G$ is adjacent to itself. 
- Second, ${} A {}$ is a  symmetric matrix, that is, row i of ${} A {}$ is identical to column $i {}$ of $A$ for every integer ${} i$ with ${} 1 ≤ i ≤ n$.
- if we were to add the entries in row ${} i$ (or in column $i$), then we obtain the degree of $v_i$.











