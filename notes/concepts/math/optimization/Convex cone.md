---
aliases:
  - Выпуклый конус
anki: true
created: 2024-10-27 22:01
parent:
  - "[[Cone set]]"
  - "[[Convex Set]]"
connected: 
tags:
---

> [!tip] Convex cone
is the set $S$, if:
$\forall x_1, x_2 \in S, \; \theta_1, \theta_2 \ge 0 \;\; \rightarrow \;\; \theta_1 x_1 + \theta_2 x_2 \in S$

![[convex_cone.svg]]

> [!EXAMPLE]
- $\mathbb{R}^n$
- Affine sets, containing $0$
- Ray
- $\mathbf{S}^n_+$ - the set of symmetric positive semi-definite matrices

> [!Important Cones]
- **Nonnegative orthant** $\mathbb{R}_+^n = \{x \in \mathbb{R}^n \mid x_i \geq 0, i = 1, \dots, n\}$ → Linear programming (LP)
- **Second-order cone** $\{(x, t) \in \mathbb{R}^{n+1} \mid \|x\|_2 \leq t\}$ → Second-order cone programming (SOCP)
- **Symmetric positive semi-definite matrices** $S_+^n$ → Semidefinite programming (SDP)


# Anki
TARGET DECK: math::optimization 
START
math_complex
FRONT: Convex cone
BACK: 
is the set $S$, if:
$\forall x_1, x_2 \in S, \; \theta_1, \theta_2 \ge 0 \;\; \rightarrow \;\; \theta_1 x_1 + \theta_2 x_2 \in S$
ADDITIONAL:
> [!EXAMPLE]
- $\mathbb{R}^n$
- Affine sets, containing $0$
- Ray
- $\mathbf{S}^n_+$ - the set of symmetric positive semi-definite matrices
PICTURE: ![[convex_cone.svg]]
ID: 1734879190929
END

TARGET DECK: math::optimization
START
math_complex
FRONT: Important Cones
BACK: 
- **Nonnegative orthant** $\mathbb{R}_+^n = \{x \in \mathbb{R}^n \mid x_i \geq 0, i = 1, \dots, n\}$ → Linear programming (LP)
- **Second-order cone** $\{(x, t) \in \mathbb{R}^{n+1} \mid \|x\|_2 \leq t\}$ → Second-order cone programming (SOCP)
- **Symmetric positive semi-definite matrices** $S_+^n$ → Semidefinite programming (SDP)
ID: 1734879278603
END