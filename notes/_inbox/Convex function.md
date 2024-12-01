---
aliases:
  - Выпуклая функция
publish: true
anki: false
created: 2024-10-27 22:20
parent:
  - "[[Function (math)]]"
  - "[[Convex Set]]"
connected:
  - "[[Concave function]]"
tags:
---

> [!tip] Function $f : \mathcal{X} \subset \mathbb{R}^n \to \mathbb{R}$ is called convex (strictly convex), 
if $\mathcal{X}$ is a convex set and $\forall \mathbf{x}_1, \mathbf{x}_2 \in \mathcal{X}$ and $\alpha \in [0, 1]$ ($\alpha \in (0, 1)$) we have: 
$f(\alpha \mathbf{x}_1 + (1 - \alpha) \mathbf{x}_2) \leq (<) \, \alpha f(\mathbf{x}_1) + (1 - \alpha) f(\mathbf{x}_2)$

##### Examples of convex functions
- $x^p$ for $x \geq 0$ and $p \geq 1$
- $x \log x$, where $x > 0$
- $\max\{x_1, \dots, x_n\}$
- $\|\mathbf{x}\|$
- $\log \left( \sum_{i=1}^n e^{x_i} \right)$
- $-\log \det \mathbf{X}$ for $\mathbf{X} \in S_{++}^n$

