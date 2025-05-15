---
aliases:
  - Конусное множество
anki: true
created: 2024-10-27 22:00
parent:
  - "[[Set (math)]]"
connected:
  - "[[Affine set]]"
  - "[[Convex Set]]"
tags:
---

> [!tip] Cone set (Geometric definition)  
is the set $\mathcal{C}$  
if for any $x \in \mathcal{C}$ and any $\lambda \geq 0$, the ray starting at the origin and passing through $x$ lies entirely in $\mathcal{C}$, i.e.  
$\forall x \in \mathcal{C}, \forall \lambda \geq 0: \lambda x \in \mathcal{C}$.

> [!tip] Cone set (Combination definition)  
is a set that is closed under all possible [[Conic combination|conic combinations]] of its points, i.e., 
$\forall x_1, x_2, \ldots, x_k \in \mathcal{C}, \forall \lambda_1, \lambda_2, \ldots, \lambda_k \geq 0$:  
$\sum\limits_{i=1}^k \lambda_i x_i \in \mathcal{C}$.

![[cone.svg]]

# Anki
TARGET DECK: math::optimization
START
Math_ONE_side
TITLE: Cone set (Geometric definition) 
DESCRIPTION: 
is the set $\mathcal{C}$  
if for any $x \in \mathcal{C}$ and any $\lambda \geq 0$, the ray starting at the origin and passing through $x$ lies entirely in $\mathcal{C}$, i.e.  
$\forall x \in \mathcal{C}, \forall \lambda \geq 0: \lambda x \in \mathcal{C}$.
PICTURE: ![[cone.svg]]
ID: 1734878207787
END

TARGET DECK: math::optimization 
START
Math_ONE_side
TITLE: Cone set (Combination definition)  
DESCRIPTION: 
is a set that is closed under all possible [[Conic combination|conic combinations]] of its points, i.e., 
$\forall x_1, x_2, \ldots, x_k \in \mathcal{C}, \forall \lambda_1, \lambda_2, \ldots, \lambda_k \geq 0$:  
$\sum\limits_{i=1}^k \lambda_i x_i \in \mathcal{C}$.
PICTURE: ![[cone.svg]]
ID: 1734878207794
END