---
aliases:
  - Выпуклая оптимизация
publish: true
created: 2024-10-17 23:20
parent:
  - "[[51 Math MOC]]"
connected: []
tags:
  - MOC
---
[[Home work 4 - Optimization]]
[[НИР]]

[[Gradient-Based Methods]]

- [[Convex Set]]
	- [[The intersection of a finite or infinite number of convex sets (theorem)]]
	- [[If the domain of any linear map is convex, then the image of this map is also convex (theorem)]]
	- Operations
		- [[The Minkowski sum of two convex sets is a convex set (theorem)]]
		- [[A linear combination of convex sets is a convex set (Corollary)]]




- [[Cone set]]
- [[Convex cone]]
- [[Convex Hull]]


- [[Convex function]] ([[Concave function]])
	- [[A function f is convex if and only if epigraph of f is a convex set (theorem)]]
	- [[Strongly Convex Function]]




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

