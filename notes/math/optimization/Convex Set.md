---
aliases:
  - Выпулкое множество
publish: true
anki: true
created: 2024-10-27 21:46
parent:
  - "[[Set (math)]]"
connected:
  - "[[Affine set]]"
  - "[[Line segment]]"
  - "[[Convex combination]]"
tags:
---

> [!tip] Convex set (geometric definition)  
is the set $\mathcal{X}$  
if for any $x_1, x_2$ from $\mathcal{X}$, the [[Line segment|line segment]] passing through them also lies in $\mathcal{X}$, i.e.  
$\forall \alpha \in [0, 1], \forall x_1, x_2 \in \mathcal{X}: \alpha x_1 + (1-\alpha) x_2 \in \mathcal{X}$.

> [!tip] Convex set (сombination definition)  
is a set that is closed under all possible [[Convex combination|convex combinations]] of its points.


| ![[Convex_polygon_illustration1.svg\|200]] | ![[Convex_polygon_illustration2.svg\|200]] |
| ------------------------------------------ | ------------------------------------------ |
| Convex set                                 | Non convex set                             |


###### Examples
- [[Polyhedron (3D)]]
- [[Hyperplane]]
- Balls in any proper norm and ellipsoids
- Set of symmetric and non-negative definite matrices


![[Affine set#Relationship between convex and affine set]]


#### Anki
> [!question]- Convex set (geometric definition)  
TARGET DECK: Math::Optimization
START
Math_TWO_side
TITLE: Convex set (geometric definition)  
DESCRIPTION: is the set $\mathcal{X}$  
if for any $x_1, x_2$ from $\mathcal{X}$, the [[Line segment|line segment]] passing through them also lies in $\mathcal{X}$, i.e.  
FORMULA: $\forall \alpha \in [0, 1], \forall x_1, x_2 \in \mathcal{X}: \alpha x_1 + (1-\alpha) x_2 \in \mathcal{X}$.
ADDITIONAL:
[[Polyhedron (3D)]]
[[Hyperplane]]
Balls in any proper norm and ellipsoids
Set of symmetric and non-negative definite matrices
PICTURE:
| ![[Convex_polygon_illustration1.svg\|200]] | ![[Convex_polygon_illustration2.svg\|200]] |
| ------------------------------------------ | ------------------------------------------ |
| Convex set                                 | Non convex set                             |
ID: 1734778303394
END

> [!question]- Convex set (сombination definition)  
TARGET DECK: Math::Optimization
START
Math_TWO_side
TITLE: Convex set (сombination definition)  
DESCRIPTION: is a set that is closed under all possible [[Convex combination|convex combinations]] of its points.
ADDITIONAL:
[[Polyhedron (3D)]]
[[Hyperplane]]
Balls in any proper norm and ellipsoids
Set of symmetric and non-negative definite matrices
PICTURE:
| ![[Convex_polygon_illustration1.svg\|200]] | ![[Convex_polygon_illustration2.svg\|200]] |
| ------------------------------------------ | ------------------------------------------ |
| Convex set                                 | Non convex set                             |
ID: 1734778303407
END
