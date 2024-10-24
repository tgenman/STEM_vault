---
aliases: 
publish: true
anki: false
created: 2024-10-17 23:25
parent: 
connected:
  - "#обс/linking"
tags:
  - empty
---

### Definition
A set $\text{epi } f = \{(x,t) \in \mathbb{R}^{n+1} \mid t \geq f(x)\}$ is called the epigraph of $f$.

### Theorem
A function $f$ is convex $\iff \text{epi } f$ is a convex set.

### Proof
1. Let $f$ be a convex function.
   - Consider any two points from the epigraph $(x_1, t_1)$ and $(x_2, t_2)$, where $t_1 \geq f(x_1)$ and $t_2 \geq f(x_2)$.
   - Check that the point $(\alpha x_1 + (1-\alpha) x_2, \alpha t_1 + (1-\alpha) t_2)$ also belongs to the epigraph.
   - From the convexity of $f$ follows $\alpha t_1 + (1-\alpha) t_2 \geq \alpha f(x_1) + (1-\alpha) f(x_2) \geq f(\alpha x_1 + (1-\alpha) x_2)$.
   
2. Let the epigraph $\text{epi } f$ be a convex set.
   - $(x_1, f(x_1))$ and $(x_2, f(x_2)) \in \text{epi } f$, then $(\alpha x_1 + (1-\alpha) x_2, \alpha f(x_1) + (1-\alpha) f(x_2)) \in \text{epi } f$.
   - From the definition of the epigraph follows the convexity of $f$.