---
aliases:
  - Сумма Минковского
publish: true
anki: true
created: 2024-10-27 21:53
parent:
  - "[[Operations on sets]]"
connected:
  - "[[Convex Set]]"
tags:
---

> [!tip] The Minkowski sum of two sets of vectors $S_1$ and $S_2$ in Euclidean space 
is formed by adding each vector in $S_1$ to each vector in $S_2$:
$S_1+S_2=\{\mathbf {s_1} +\mathbf {s_2} \,|\,\mathbf {s_1} \in S_1,\ \mathbf {s_2} \in S_2\}$



![[Сумма_Минковского.svg|300]]
The red figure is the Minkowski sum of blue and green figures.


#### Theorem
> [!tip] theorem
The [[Minkowski sum]] of two convex sets is a convex set (theorem)

##### Proof
- Let $\mathcal{X}_1, \mathcal{X}_2$ be convex sets. Consider $\mathcal{X} = \mathcal{X}_1 + \mathcal{X}_2 = \{x_1 + x_2 \mid x_1 \in \mathcal{X}_1, x_2 \in \mathcal{X}_2\}$.
- Let $\hat{x} = \hat{x}_1 + \hat{x}_2$ and $\tilde{x} = \tilde{x}_1 + \tilde{x}_2$ belong to $\mathcal{X}$. Show that $\alpha \hat{x} + (1-\alpha) \tilde{x} \in \mathcal{X}$.
  
Indeed, $\alpha \hat{x} + (1-\alpha) \tilde{x} = [\alpha \hat{x}_1 + (1-\alpha) \tilde{x}_1] + [\alpha \hat{x}_2 + (1-\alpha) \tilde{x}_2] = y_1 + y_2,$ where $y_1 \in \mathcal{X}_1$ and $y_2 \in \mathcal{X}_2$, since sets $\mathcal{X}_1, \mathcal{X}_2$ are convex.

#### Anki
> [!question]- The Minkowski sum of two sets of vectors $S_1$ and $S_2$ in Euclidean space 
TARGET DECK: Math::Optimization
START
Math_ONE_side
TITLE: The Minkowski sum of two sets of vectors $S_1$ and $S_2$ in Euclidean space 
DESCRIPTION: is formed by adding each vector in $S_1$ to each vector in $S_2$:
$S_1+S_2=\{\mathbf {s_1} +\mathbf {s_2} \,|\,\mathbf {s_1} \in S_1,\ \mathbf {s_2} \in S_2\}$
FORMULA: 
ADDITIONAL:
PICTURE: ![[Сумма_Минковского.svg|300]]
The red figure is the Minkowski sum of blue and green figures.
ID: 1734859945756
END

> [!question]- Theorem about Minkowski sum
TARGET DECK: Math::Optimization
START
Math_ONE_side
TITLE: 
DESCRIPTION: The [[Minkowski sum]] of two convex sets is a convex set (theorem)
ADDITIONAL:
Proof
Let $\mathcal{X}_1, \mathcal{X}_2$ be convex sets. Consider $\mathcal{X} = \mathcal{X}_1 + \mathcal{X}_2 = \{x_1 + x_2 \mid x_1 \in \mathcal{X}_1, x_2 \in \mathcal{X}_2\}$.
Let $\hat{x} = \hat{x}_1 + \hat{x}_2$ and $\tilde{x} = \tilde{x}_1 + \tilde{x}_2$ belong to $\mathcal{X}$. Show that $\alpha \hat{x} + (1-\alpha) \tilde{x} \in \mathcal{X}$.
Indeed, $\alpha \hat{x} + (1-\alpha) \tilde{x} = [\alpha \hat{x}_1 + (1-\alpha) \tilde{x}_1] + [\alpha \hat{x}_2 + (1-\alpha) \tilde{x}_2] = y_1 + y_2,$ where $y_1 \in \mathcal{X}_1$ and $y_2 \in \mathcal{X}_2$, since sets $\mathcal{X}_1, \mathcal{X}_2$ are convex.
PICTURE: ![[Сумма_Минковского.svg|300]]
ID: 1734859945763
END