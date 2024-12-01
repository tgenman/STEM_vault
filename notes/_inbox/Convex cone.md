---
aliases:
  - Выпуклый конус
publish: true
anki: false
created: 2024-10-27 22:01
parent:
  - "[[Cone set]]"
  - "[[Convex Set]]"
connected:
  - "#обс/linking"
tags: []
---

> [!tip] A set $\mathcal{K}$ is called a **convex cone** 
> if for any points $x_1, x_2 \in \mathcal{K}$ and any numbers $\theta_1 \geq 0$, $\theta_2 \geq 0$, we have $\theta_1 x_1 + \theta_2 x_2 \in \mathcal{K}$.

#### Important Cones
- **Nonnegative orthant** $\mathbb{R}_+^n = \{x \in \mathbb{R}^n \mid x_i \geq 0, i = 1, \dots, n\}$ → Linear programming (LP)
- **Second-order cone** $\{(x, t) \in \mathbb{R}^{n+1} \mid \|x\|_2 \leq t\}$ → Second-order cone programming (SOCP)
- **Symmetric positive semi-definite matrices** $S_+^n$ → Semidefinite programming (SDP)

