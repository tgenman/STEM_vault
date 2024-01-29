---
aliases: 
publish: true
anki: true
created: 2023-11-15 14:58
parent:
  - "[[Irregular graph]]"
connected:
  - "[[Degree Sequence]]"
tags:
  - theorem
---

> [!note] 
No graph is irregular

#### Proof
Proof. Assume, to the contrary, that there exists an irregular graph $G$ of order $n \geq 2$. Since the degree of every vertex of $G$ is one of the $n$ integers $0, 1, \ldots, n - 1$, each of these integers is the degree of exactly one vertex. Thus, we may assume that $V(G) = \{v_1, v_2, \ldots, v_n\}$ where $\deg v_i = i - 1$ for $1 \leq i \leq n$. Since $\deg v_1 = 0$, the vertex $v_1$ is isolated in $G$ and since $\deg v_n = n - 1$, it follows that $v_n$ is adjacent to $v_1$. This is a contradiction. 

#### Anki
> [!question]- Theorem about no existence irregular graph
TARGET DECK: Math::Graph 
START
Math_ONE_side
TITLE:  Theorem about no existence irregular graph
DESCRIPTION: No graph is irregular
FORMULA: Proof
Proof. Assume, to the contrary, that there exists an irregular graph $G$ of order $n \geq 2$. Since the degree of every vertex of $G$ is one of the $n$ integers $0, 1, \ldots, n - 1$, each of these integers is the degree of exactly one vertex. Thus, we may assume that $V(G) = \{v_1, v_2, \ldots, v_n\}$ where $\deg v_i = i - 1$ for $1 \leq i \leq n$. Since $\deg v_1 = 0$, the vertex $v_1$ is isolated in $G$ and since $\deg v_n = n - 1$, it follows that $v_n$ is adjacent to $v_1$. This is a contradiction. 
ADDITIONAL:
ID: 1705602014663
END











