---
aliases:
  - Умножение матрицы на скаляр
anki: true
created: 2024-04-16 19:30
parent:
  - "[[Matrix Operations]]"
connected: 
tags:
---

Let $A \in \mathbb{R}^{m \times n}$ and $\lambda \in \mathbb{R}$. 
Then $\lambda A = K$, $K_{ij} = \lambda a_{ij}$. Practically, $\lambda$ scales each element of $A$. 
For $\lambda, \psi \in \mathbb{R}$, the following holds:
Associativity:
- Associativity: $(\lambda\psi)C = \lambda(\psi C)$, where $C \in \mathbb{R}^{m \times n}$
- $\lambda(BC) = (\lambda B)C = B(\lambda C)$, where $B \in \mathbb{R}^{m \times n}$, $C \in \mathbb{R}^{n \times k}$. Note that this allows us to move scalar values around.
- $(\lambda C)^T = C^T \lambda^T = C^T \lambda$ since $\lambda = \lambda^T$ for all $\lambda \in \mathbb{R}$.

Distributivity:
- Distributivity: $(\lambda + \psi)C = \lambda C + \psi C$, where $C \in \mathbb{R}^{m \times n}$
- $\lambda(B + C) = \lambda B + \lambda C$, where $B, C \in \mathbb{R}^{m \times n}$


# Anki
TARGET DECK: math::linal 
START
math_complex
FRONT: Properties Matrix Scalar Multiplication
BACK: 
Let $A \in \mathbb{R}^{m \times n}$ and $\lambda \in \mathbb{R}$. 
Then $\lambda A = K$, $K_{ij} = \lambda a_{ij}$. Practically, $\lambda$ scales each element of $A$. 
For $\lambda, \psi \in \mathbb{R}$, the following holds:
Associativity:
- Associativity: $(\lambda\psi)C = \lambda(\psi C)$, where $C \in \mathbb{R}^{m \times n}$
- $\lambda(BC) = (\lambda B)C = B(\lambda C)$, where $B \in \mathbb{R}^{m \times n}$, $C \in \mathbb{R}^{n \times k}$. Note that this allows us to move scalar values around.
- $(\lambda C)^T = C^T \lambda^T = C^T \lambda$ since $\lambda = \lambda^T$ for all $\lambda \in \mathbb{R}$.
Distributivity:
- Distributivity: $(\lambda + \psi)C = \lambda C + \psi C$, where $C \in \mathbb{R}^{m \times n}$
- $\lambda(B + C) = \lambda B + \lambda C$, where $B, C \in \mathbb{R}^{m \times n}$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1713287496938
END
