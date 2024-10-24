---
aliases: 
publish: true
created: 2024-10-17 23:20
parent:
  - "[[51 Math MOC]]"
connected:
  - "#обс/linking"
tags:
  - empty
---

## Convex Sets

### Definition
A set $\mathcal{X} \subseteq \mathbb{R}^n$ is convex if for all $\alpha \in [0, 1]$ and for any $x, y \in \mathcal{X}$, the following holds:
$$\alpha x + (1-\alpha) y \in \mathcal{X}.$$

### Examples
- Polyhedron
- Hyperplanes
- Balls in any proper norm and ellipsoids
- Set of symmetric and non-negative definite matrices

## Intersection of Convex Sets

### Theorem
The intersection of a finite or infinite number of convex sets $X_i$ is a convex set:
$$\mathcal{X} = \bigcap_{i \in I} X_i.$$

### Proof
- Consider $x, y \in \mathcal{X} \Rightarrow x, y \in X_i, \forall i \in I$.
- Consider the point $z = \alpha x + (1-\alpha) y$, $\alpha \in [0, 1]$.
- Since $X_i$ is convex for all $i \in I$, $z \in X_i, \forall i \in I$.
- Therefore, $z \in \mathcal{X}$ and $\mathcal{X}$ is a convex set.


## Linear Map of Convex Set

### Theorem
If the domain of any linear map is convex, then the image of this map is also convex.

### Proof
- Let $\mathcal{X}$ be a convex set and $x, y \in \mathcal{X}$.
- Let $f$ be a linear map: $f(x) = A x + b$.
- Show that $\alpha f(x) + (1-\alpha) f(y) \in f(\mathcal{X})$, where $\alpha \in [0, 1]$.

Indeed,
$$\alpha f(x) + (1-\alpha) f(y) = \alpha (A x + b) + (1-\alpha) (A y + b) = A (\alpha x + (1-\alpha) y) + b = f(z),$$
where $z = \alpha x + (1-\alpha) y \in \mathcal{X}$.

## Arithmetic Operations under Convex Sets

### Theorem
The Minkowski sum of two convex sets is a convex set.

### Proof
- Let $\mathcal{X}_1, \mathcal{X}_2$ be convex sets. Consider $\mathcal{X} = \mathcal{X}_1 + \mathcal{X}_2 = \{x_1 + x_2 \mid x_1 \in \mathcal{X}_1, x_2 \in \mathcal{X}_2\}$.
- Let $\hat{x} = \hat{x}_1 + \hat{x}_2$ and $\tilde{x} = \tilde{x}_1 + \tilde{x}_2$ belong to $\mathcal{X}$. Show that $\alpha \hat{x} + (1-\alpha) \tilde{x} \in \mathcal{X}$.
  
Indeed,
$$\alpha \hat{x} + (1-\alpha) \tilde{x} = [\alpha \hat{x}_1 + (1-\alpha) \tilde{x}_1] + [\alpha \hat{x}_2 + (1-\alpha) \tilde{x}_2] = y_1 + y_2,$$
where $y_1 \in \mathcal{X}_1$ and $y_2 \in \mathcal{X}_2$, since sets $\mathcal{X}_1, \mathcal{X}_2$ are convex.

### Corollary
A linear combination of convex sets is a convex set.

## Cones

### Definition
A set $\mathcal{K}$ is a cone if for any $x \in \mathcal{K}$ and arbitrary number $\theta \geq 0$, we have $\theta x \in \mathcal{K}$.

### Definition
A set $\mathcal{K}$ is called a **convex cone** if for any points $x_1, x_2 \in \mathcal{K}$ and any numbers $\theta_1 \geq 0$, $\theta_2 \geq 0$, we have $\theta_1 x_1 + \theta_2 x_2 \in \mathcal{K}$.

### Important Cones
- **Nonnegative orthant** $\mathbb{R}_+^n = \{x \in \mathbb{R}^n \mid x_i \geq 0, i = 1, \dots, n\}$ → Linear programming (LP)
- **Second-order cone** $\{(x, t) \in \mathbb{R}^{n+1} \mid \|x\|_2 \leq t\}$ → Second-order cone programming (SOCP)
- **Symmetric positive semi-definite matrices** $S_+^n$ → Semidefinite programming (SDP)


## Convex Hull

### Definition
The convex hull of the set $\mathcal{G}$ is called the set $\text{conv}(\mathcal{G})$ that:
- It is an intersection of all convex sets containing $\mathcal{G}$.
- It is a set of all convex combinations of points from $\mathcal{G}$:
  $$\text{conv}(\mathcal{G}) = \left\{ \sum_{i=1}^{k} \theta_i x_i \mid x_i \in \mathcal{G}, \sum_{i=1}^{k} \theta_i = 1, \theta_i \geq 0 \right\}$$
- It is the minimal convex set containing $\mathcal{G}$.
  













[[Epigraph of function]]

## Strongly Convex Function

### Definition
A function $f : \mathcal{X} \subset \mathbb{R}^n \to \mathbb{R}$ is called strongly convex with constant $m > 0$, if $\mathcal{X}$ is a convex set and $\forall x_1, x_2 \in \mathcal{X}$ and $\alpha \in [0, 1]$, we have:
$$f(\alpha x_1 + (1-\alpha) x_2) \leq \alpha f(x_1) + (1-\alpha) f(x_2) - \frac{m}{2} \alpha (1-\alpha) \|x_1 - x_2\|_2^2$$

- Convexity $\supset$ strict convexity $\supset$ strong convexity.
- Theoretical analysis of methods in the case of strongly convex functions significantly differs from the one for convex functions.


## Gradient and Hessian: Preliminaries

Consider $f : \mathbb{R}^n \to \mathbb{R}$.

- **Directional derivative**:
  $$f'_d(x) = \lim_{\alpha \to 0} \frac{f(x + \alpha d) - f(x)}{\alpha}$$

- **Gradient** $f'(x)$ is a vector such that $\left[f'(x)\right]_i = \frac{\partial f}{\partial x_i}$.

- **Hessian** is a square matrix $f''(x)$ such that $\left[f''(x)\right]_{ij} = \frac{\partial^2 f}{\partial^2 x_i \partial^2 x_j}$.


## Differential Criteria of Convexity

We consider a convex function as a strongly convex function with $m = 0$.

### Theorem (First-order criterion)
Let a function $f(x)$ be differentiable and its domain be a convex set $\mathcal{X} \subseteq \mathbb{R}^n$. Then $f(x)$ is strongly convex with $m \geq 0$ if and only if:
$$f(x) - f(x^*) \geq \langle f'(x^*), x - x^* \rangle + \frac{m}{2} \|x - x^*\|_2^2, \quad \forall x, x^* \in \mathcal{X}.$$


![[Pasted image 20241017233914.png|400]]


### Theorem (Second-order criterion)
A twice continuously differentiable function $f$ is convex if and only if:
$$f''(x) \succeq m \mathbf{I}$$

## What Function Compositions Preserve Convexity?

- If $f(x)$ is convex, then $g(x) = f(Ax + b)$ is convex.
- If $f(x)$ is convex, then $g(t) = f(x + t y)$ is convex.
- If $f_i(x)$ are convex, then $f(x) = \max_{i=1,\dots,m} f_i(x)$ is convex.
- The sum of convex functions with non-negative coefficients is a convex function.
- Scalar composition $h(f(x))$ preserves convexity under certain conditions.


## Local Minimum of Convex Function is also a Global Minimum

### Theorem
If $f$ is a convex function and $x^*$ is a point of local minimum, then $x^*$ is a point of global minimum.

### Proof
- Assume that there exists a point $y^*$ such that $y^* \neq x^*$ and $y^*$ is a point of global minimum: $f(y^*) < f(x^*)$.
- By the definition of a point of local minimum: $f(x^*) \leq f(x)$, where $\|x^* - x\|_2 \leq \delta$.
- Choose sufficiently small $\alpha \in (0, 1)$ and consider a point $z = (1-\alpha) x^* + \alpha y^*$ such that $\|x^* - z\|_2 \leq \delta$.
- $$f(x^*) \leq f(z) \leq \alpha f(y^*) + (1-\alpha) f(x^*) < f(x^*).$$
- We get a contradiction, therefore the assumption is incorrect and $x^*$ is a point of global minimum.




[[Jensen Inequality]]
[[Cauchy-Schwarz-Буняковского Inequality]]
[[Holder's Inequality]]

