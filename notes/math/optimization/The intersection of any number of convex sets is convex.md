---
aliases: 
anki: true
created: 2024-12-23 22:40
parent:
  - "[[Operations preserving convexity]]"
connected:
  - "[[Intersection of Sets (A ∩ B)]]"
tags:
---

> [!tip] 
The intersection of a finite or infinite number of convex sets $X_i$ is a convex set:
$\mathcal{X} = \bigcap_{i \in I} X_i$

##### Proof
- Consider $x, y \in \mathcal{X} \Rightarrow x, y \in X_i, \forall i \in I$.
- Consider the point $z = \alpha x + (1-\alpha) y$, $\alpha \in [0, 1]$.
- Since $X_i$ is convex for all $i \in I$, $z \in X_i, \forall i \in I$.
- Therefore, $z \in \mathcal{X}$ and $\mathcal{X}$ is a convex set.

#### Anki
> [!question]- The intersection of any number of convex sets is convex
TARGET DECK: math::optimization
START
Math_ONE_side
TITLE: The intersection of any number of convex sets is 
DESCRIPTION: convex
The intersection of a finite or infinite number of convex sets $X_i$ is a convex set:
$\mathcal{X} = \bigcap_{i \in I} X_i$
ADDITIONAL:
Consider $x, y \in \mathcal{X} \Rightarrow x, y \in X_i, \forall i \in I$.
Consider the point $z = \alpha x + (1-\alpha) y$, $\alpha \in [0, 1]$.
Since $X_i$ is convex for all $i \in I$, $z \in X_i, \forall i \in I$.
Therefore, $z \in \mathcal{X}$ and $\mathcal{X}$ is a convex set.
ID: 1734968542485
END
