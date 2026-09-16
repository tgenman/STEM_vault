---
aliases:
  - Сильно выпуклая функция
anki: false
created: 2024-10-27 22:26
parent:
  - "[[Convex function]]"
connected: []
tags:
---

> [!tip] A function $f : \mathcal{X} \subset \mathbb{R}^n \to \mathbb{R}$ is called strongly convex with constant $m > 0$, 
if $\mathcal{X}$ is a [[Convex Set|convex set]]  and $\forall x_1, x_2 \in \mathcal{X}$ and $\alpha \in [0, 1]$, we have:
$f(\alpha x_1 + (1-\alpha) x_2) \leq \alpha f(x_1) + (1-\alpha) f(x_2) - \frac{m}{2} \alpha (1-\alpha) \|x_1 - x_2\|_2^2$


- Strong convexity with $m>0$ implies [[strictly convex function|strict convexity]], which implies [[Convex function|convexity]]. The converses do not hold in general.
- Setting $m=0$ in the inequality gives ordinary convexity; it is not strong convexity with a positive constant.
- Theoretical analysis of methods in the case of strongly convex functions significantly differs from the one for convex functions.

- [[first-order criterion of convexity]]
- [[second-order criterion of convexity]]
