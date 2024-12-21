---
aliases:
  - Выпулкая оболочка
publish: true
anki: false
created: 2024-10-27 22:03
parent:
  - "[[Convex Set]]"
connected:
  - "[[Span|Линейная оболочка]]"
tags:
---

> [!tip] The convex hull of the set $\mathcal{G}$ is called the set $\text{conv}(\mathcal{G})$ that:
> - It is an intersection of all convex sets containing $\mathcal{G}$.
> - It is a set of all convex combinations of points from $\mathcal{G}$:
  $\text{conv}(\mathcal{G}) = \left\{ \sum_{i=1}^{k} \theta_i x_i \mid x_i \in \mathcal{G}, \sum_{i=1}^{k} \theta_i = 1, \theta_i \geq 0 \right\}$
> - It is the minimal convex set containing $\mathcal{G}$.


![[ConvexHull.svg]]
