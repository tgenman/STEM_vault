---
aliases: 
anki: false
created: 2024-10-27 21:49
parent:
  - "[[Convex Set]]"
connected:
  - "#обс/linking"
tags:
  - content/theorem
---

> [!tip] 
The intersection of a finite or infinite number of convex sets $X_i$ is a convex set:
$\mathcal{X} = \bigcap_{i \in I} X_i$

##### Proof
- Consider $x, y \in \mathcal{X} \Rightarrow x, y \in X_i, \forall i \in I$.
- Consider the point $z = \alpha x + (1-\alpha) y$, $\alpha \in [0, 1]$.
- Since $X_i$ is convex for all $i \in I$, $z \in X_i, \forall i \in I$.
- Therefore, $z \in \mathcal{X}$ and $\mathcal{X}$ is a convex set.