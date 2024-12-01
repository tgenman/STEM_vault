---
aliases: 
publish: true
anki: false
created: 2024-10-27 21:53
parent:
  - "[[Convex Set]]"
  - "[[Minkowski sum]]"
connected:
  - "#обс/linking"
tags:
  - theorem
---

> [!tip] theorem
The [[Minkowski sum]] of two convex sets is a convex set (theorem)

#### Proof
- Let $\mathcal{X}_1, \mathcal{X}_2$ be convex sets. Consider $\mathcal{X} = \mathcal{X}_1 + \mathcal{X}_2 = \{x_1 + x_2 \mid x_1 \in \mathcal{X}_1, x_2 \in \mathcal{X}_2\}$.
- Let $\hat{x} = \hat{x}_1 + \hat{x}_2$ and $\tilde{x} = \tilde{x}_1 + \tilde{x}_2$ belong to $\mathcal{X}$. Show that $\alpha \hat{x} + (1-\alpha) \tilde{x} \in \mathcal{X}$.
  
Indeed,
$$\alpha \hat{x} + (1-\alpha) \tilde{x} = [\alpha \hat{x}_1 + (1-\alpha) \tilde{x}_1] + [\alpha \hat{x}_2 + (1-\alpha) \tilde{x}_2] = y_1 + y_2,$$
where $y_1 \in \mathcal{X}_1$ and $y_2 \in \mathcal{X}_2$, since sets $\mathcal{X}_1, \mathcal{X}_2$ are convex.