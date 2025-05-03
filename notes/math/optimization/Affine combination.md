---
aliases:
  - Афинная комбинация
anki: true
created: 2024-12-19 23:39
parent:
  - "[[Affine set]]"
connected:
  - "[[Linear combination]]"
  - "[[Convex combination]]"
  - "[[Conic combination]]"
tags:
---
 
> [!tip] Affine combination
for $x_1, x_2, \ldots, x_k \in S$ and $\theta_1, \theta_2, \ldots, \theta_k \in \mathbb{R}$  
is the point $\theta_1 x_1 + \theta_2 x_2 + \ldots + \theta_k x_k$ 
if $\sum\limits_{i=1}^k\theta_i = 1$.


#### Difference between conic, convex, affine, and linear combinations

##### Hierarchy-based Comparison
[[Convex combination]] $\subseteq$ [[Affine combination]] $\subseteq$ [[Linear combination]]  
[[Convex combination]] $\subseteq$ [[Conic combination]] $\subseteq$ [[Linear combination]]

##### Property-based Table
| Combination Type       | Restriction on $\sum\limits_{i=1}^n \alpha_i$ | Restriction on $\alpha_i$     |
| ---------------------- | --------------------------------------------- | ----------------------------- |
| [[Linear combination]] | No restriction                                | No restriction                |
| [[Affine combination]] | $\sum\limits_{i=1}^n \alpha_i = 1$            | No restriction                |
| [[Convex combination]] | $\sum\limits_{i=1}^n \alpha_i = 1$            | $\alpha_i \geq 0$ for all $i$ |
| [[Conic combination]]  | No restriction                                | $\alpha_i \geq 0$ for all $i$ |

##### Matrix-based Categorization
|                   | $\sum \alpha_i = 1$    | No restriction         |
| ----------------- | ---------------------- | ---------------------- |
| $\alpha_i \geq 0$ | [[Convex combination]] | [[Conic combination]]  |
| No restriction    | [[Affine combination]] | [[Linear combination]] |


#### Difference between Convex and Afiine combination on graph
![[Convex_combination_illustration.svg|200]]
Given three points ${x_1}$, ${x_2}$, ${x_3}$ on a plane. The point $P$ is a [[Convex combination]] of these three points, whereas $Q$ is not.
($Q$, however, is an [[Affine combination]] of these three vectors since their [[Affine hull - aff(S)]] coincides with the entire plane.)



#### Anki
> [!question]- Affine combination
TARGET DECK: Math::Optimization
START
Math_TWO_side
TITLE: Affine combination
DESCRIPTION: for $x_1, x_2, \ldots, x_k \in S$ and $\theta_1, \theta_2, \ldots, \theta_k \in \mathbb{R}$  
is the point $\theta_1 x_1 + \theta_2 x_2 + \ldots + \theta_k x_k$ 
if $\sum\limits_{i=1}^k\theta_i = 1$.
ID: 1734779669666
END

> [!question]- Difference between conic, convex, affine, and linear combinations. Hierarchy-based Comparison
TARGET DECK: Math::Optimization
START
Math_ONE_side
TITLE: Difference between conic, convex, affine, and linear combinations. Hierarchy-based Comparison
DESCRIPTION: 
[[Convex combination]] $\subseteq$ [[Affine combination]] $\subseteq$ [[Linear combination]]  
[[Convex combination]] $\subseteq$ [[Conic combination]] $\subseteq$ [[Linear combination]]
ID: 1734763705921
END

> [!question]- Difference between conic, convex, affine, and linear combinations. Property-based Table
TARGET DECK: Math::Optimization
START
Math_ONE_side
TITLE: Difference between conic, convex, affine, and linear combinations. Property-based Table
DESCRIPTION:
| Combination Type       | Restriction on $\sum\limits_{i=1}^n \alpha_i$ | Restriction on $\alpha_i$     |
| ---------------------- | --------------------------------------------- | ----------------------------- |
| [[Linear combination]] | No restriction                                | No restriction                |
| [[Affine combination]] | $\sum\limits_{i=1}^n \alpha_i = 1$            | No restriction                |
| [[Convex combination]] | $\sum\limits_{i=1}^n \alpha_i = 1$            | $\alpha_i \geq 0$ for all $i$ |
| [[Conic combination]]  | No restriction                                | $\alpha_i \geq 0$ for all $i$ |
ID: 1734779794045
END

> [!question]- Difference between conic, convex, affine, and linear combinations. Matrix-based Categorization
TARGET DECK: Math::Optimization
START
Math_ONE_side
TITLE: Difference between conic, convex, affine, and linear combinations. Matrix-based Categorization
DESCRIPTION:
|                   | $\sum \alpha_i = 1$    | No restriction         |
| ----------------- | ---------------------- | ---------------------- |
| $\alpha_i \geq 0$ | [[Convex combination]] | [[Conic combination]]  |
| No restriction    | [[Affine combination]] | [[Linear combination]] |
ID: 1734779794055
END

> [!question]- Difference between Convex and Afiine combination on graph
TARGET DECK: Math::Optimization
START
Math_ONE_side
TITLE: Difference between Convex and Afiine combination on graph
DESCRIPTION: Given three points ${x_1}$, ${x_2}$, ${x_3}$ on a plane. The point $P$ is a [[Convex combination]] of these three points, whereas $Q$ is not.
($Q$, however, is an [[Affine combination]] of these three vectors since their [[Affine hull - aff(S)]] coincides with the entire plane.)
FORMULA: 
ADDITIONAL:
PICTURE: ![[Convex_combination_illustration.svg|200]]
ID: 1734781570235
END
