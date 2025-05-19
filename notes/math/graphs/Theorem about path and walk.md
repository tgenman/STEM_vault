---
aliases: 
parent:
  - "[[Path P]]"
  - "[[Walk W]]"
connected: 
tags:
  - theorem
---

> [!note] Theorem about path and walk
Let $u$ and $v$ be two vertices of a graph $G$. For every $u − v$ [[Walk W|walk]]  $W$ in $G,$ there exists a $u−v$ [[Path P|path]] $P$ such that every edge of $P$ belongs to$ W$.

### Proof. 
Let $W$ be a $u - v$ walk. Among all $u - v$ walks in $G$, every edge of which belongs to $W$, let

$$ P = (u = u_0, u_1, ..., u_k = v) $$

be one of minimum length. Thus, the length of $P$ is $k$. We claim that $P$ is a $u - v$ path. Assume, to the contrary, that this is not the case. Then some vertex of $G$ must be repeated in $P$, say $u_i = u_j$ for some $i$ and $j$ with $0 \leq i < j \leq k$. If we then delete the vertices $u_{i+1}, u_{i+2}, ..., u_j$ from $P$, we arrive at the $u - v$ walk

$$ W' = (u = u_0, u_1, ..., u_{i-1}, u_i = u_j, u_{j+1}, ..., u_k = v) $$

whose length is less than $k$ and such that every edge of $W'$ belongs to $W$. This is a contradiction.

# Anki
TARGET DECK: math::graph
START
math_complex
FRONT: Theorem about path and walk
BACK: Let $u$ and $v$ be two vertices of a graph $G$. For every $u − v$ [[Walk W|walk]]  $W$ in $G,$ there exists a $u−v$ [[Path P|path]] $P$ such that every edge of $P$ belongs to$ W$.
FORMULA: ### Proof. 
Let $W$ be a $u - v$ walk. Among all $u - v$ walks in $G$, every edge of which belongs to $W$, let

$$ P = (u = u_0, u_1, ..., u_k = v) $$

be one of minimum length. Thus, the length of $P$ is $k$. We claim that $P$ is a $u - v$ path. Assume, to the contrary, that this is not the case. Then some vertex of $G$ must be repeated in $P$, say $u_i = u_j$ for some $i$ and $j$ with $0 \leq i < j \leq k$. If we then delete the vertices $u_{i+1}, u_{i+2}, ..., u_j$ from $P$, we arrive at the $u - v$ walk

$$ W' = (u = u_0, u_1, ..., u_{i-1}, u_i = u_j, u_{j+1}, ..., u_k = v) $$

whose length is less than $k$ and such that every edge of $W'$ belongs to $W$. This is a contradiction.
ADDITIONAL:
ID: 1705601974450
END












