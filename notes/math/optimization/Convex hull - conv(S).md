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
  - "[[Affine hull - aff(S)]]"
tags: 
---

> [!tip] The convex hull of the set $S$ is called the set $\text{conv}(S)$ that:
> - It is a set of all [[Convex combination]] of points from $S$:
  $\text{conv}(S) = \left\{ \sum_{i=1}^{k} \theta_i x_i \mid x_i \in S, \sum_{i=1}^{k} \theta_i = 1, \theta_i \geq 0 \right\}$
> - It is an intersection of all convex sets containing $S$.
> - It is the minimal convex set containing $S$
> - The set $S$ is convex if and only if $S = \mathbf{conv}(S)$.


![[ConvexHull.svg]]


| ![[convex_sets.svg]] | ![[convex_hull.svg]] |
| -------------------- | -------------------- |
| Different sets       | Their Convex Hull    |

#### Anki
> [!question]- Convex hull conv(S)
TARGET DECK: Math::Optimization
START
Math_ONE_side
TITLE: Convex hull conv(S)
DESCRIPTION: 
> - It is a set of all [[Convex combination]] of points from $S$:
  $\text{conv}(S) = \left\{ \sum_{i=1}^{k} \theta_i x_i \mid x_i \in S, \sum_{i=1}^{k} \theta_i = 1, \theta_i \geq 0 \right\}$
> - It is an intersection of all convex sets containing $S$.
> - It is the minimal convex set containing $S$
> - The set $S$ is convex if and only if $S = \mathbf{conv}(S)$.
FORMULA: 
ADDITIONAL:
| ![[convex_sets.svg]] | ![[convex_hull.svg]] |
| -------------------- | -------------------- |
| Different sets       | Their Convex Hull    |
PICTURE: ![[ConvexHull.svg]]
ID: 1734859099712
END