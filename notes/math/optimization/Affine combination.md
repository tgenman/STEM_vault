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



# Anki
TARGET DECK: math::optimization
START
Math_TWO_side
FRONT: Affine combination
BACK: for $x_1, x_2, \ldots, x_k \in S$ and $\theta_1, \theta_2, \ldots, \theta_k \in \mathbb{R}$  
is the point $\theta_1 x_1 + \theta_2 x_2 + \ldots + \theta_k x_k$ 
if $\sum\limits_{i=1}^k\theta_i = 1$.
ID: 1734779669666
END

TARGET DECK: math::optimization
START
math_complex
FRONT: Difference between conic, convex, affine, and linear combinations. Hierarchy-based Comparison
BACK: 
[[Convex combination]] $\subseteq$ [[Affine combination]] $\subseteq$ [[Linear combination]]  
[[Convex combination]] $\subseteq$ [[Conic combination]] $\subseteq$ [[Linear combination]]
ID: 1734763705921
END

TARGET DECK: math::optimization
START
math_complex
FRONT: Difference between conic, convex, affine, and linear combinations. Property-based Table
BACK:
| Combination Type       | Restriction on $\sum\limits_{i=1}^n \alpha_i$ | Restriction on $\alpha_i$     |
| ---------------------- | --------------------------------------------- | ----------------------------- |
| [[Linear combination]] | No restriction                                | No restriction                |
| [[Affine combination]] | $\sum\limits_{i=1}^n \alpha_i = 1$            | No restriction                |
| [[Convex combination]] | $\sum\limits_{i=1}^n \alpha_i = 1$            | $\alpha_i \geq 0$ for all $i$ |
| [[Conic combination]]  | No restriction                                | $\alpha_i \geq 0$ for all $i$ |
ID: 1734779794045
END

TARGET DECK: math::optimization
START
math_complex
FRONT: Difference between conic, convex, affine, and linear combinations. Matrix-based Categorization
BACK:
|                   | $\sum \alpha_i = 1$    | No restriction         |
| ----------------- | ---------------------- | ---------------------- |
| $\alpha_i \geq 0$ | [[Convex combination]] | [[Conic combination]]  |
| No restriction    | [[Affine combination]] | [[Linear combination]] |
ID: 1734779794055
END

TARGET DECK: math::optimization
START
math_complex
FRONT: Difference between Convex and Afiine combination on graph
BACK: Given three points ${x_1}$, ${x_2}$, ${x_3}$ on a plane. The point $P$ is a [[Convex combination]] of these three points, whereas $Q$ is not.
($Q$, however, is an [[Affine combination]] of these three vectors since their [[Affine hull - aff(S)]] coincides with the entire plane.)
FORMULA: 
ADDITIONAL:
PICTURE: ![[Convex_combination_illustration.svg|200]]
ID: 1734781570235
END
