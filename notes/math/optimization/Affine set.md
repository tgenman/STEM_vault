---
aliases:
  - Афинное множество
anki: true
created: 2024-12-19 23:27
parent:
  - "[[Set (math)]]"
connected:
  - "[[Affine combination]]"
  - "[[Convex Set]]"
  - "[[Cone set]]"
tags:
---

> [!tip] Affine set (geometric definition)
is the set $A$ 
if for any $x_1, x_2$ from $A$ the [[Line|line]]  passing through them also lies in $A$, i.e. 
$\forall \theta \in \mathbb{R}, \forall x_1, x_2 \in A: \theta x_1 + (1- \theta) x_2 \in A$

> [!tip] Affine set (сombination definition)
is a set that is closed under all possible [[Affine combination|affine combinations]]  of its points.

> [!EXAMPLE]
> - $\mathbb{R}^n$ is an affine set.
> - The set of solutions $\left\{x \mid \mathbf{A}x =  \mathbf{b} \right\}$ is also an affine set.


#### Relationship between convex and affine set
[[Convex Set]] $\subseteq$  [[Affine set]]  


# Anki
TARGET DECK: math::optimization
START
Math_TWO_side
TITLE: Affine set (geometric definition)
DESCRIPTION: is the set $A$ 
if for any $x_1, x_2$ from $A$ the [[Line|line]]  passing through them also lies in $A$, i.e. 
FORMULA: $\forall \theta \in \mathbb{R}, \forall x_1, x_2 \in A: \theta x_1 + (1- \theta) x_2 \in A$
ADDITIONAL:
$\mathbb{R}^n$ is an affine set.
The set of solutions $\left\{x \mid \mathbf{A}x =  \mathbf{b} \right\}$ is also an affine set.
ID: 1734778183469
END

TARGET DECK: math::optimization
START
Math_TWO_side
TITLE: Affine set (сombination definition)
DESCRIPTION: is a set that is closed under all possible [[Affine combination|affine combinations]]  of its points.
ADDITIONAL:
$\mathbb{R}^n$ is an affine set.
The set of solutions $\left\{x \mid \mathbf{A}x =  \mathbf{b} \right\}$ is also an affine set.
ID: 1734778183475
END

TARGET DECK: math::optimization
START
Math_ONE_side
TITLE: Relationship between convex and affine set
FORMULA: [[Convex Set]] $\subseteq$  [[Affine set]]  
ID: 1734778183480
END
