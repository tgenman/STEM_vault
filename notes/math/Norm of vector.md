---
aliases:
  - Норма вектора
publish: true
created: 2024-02-03 17:59
parent:
  - "[[Vector|Вектор]]"
anki: false
connected:
  - "[[Unit vector]]"
tags:
  - empty
---

> [!tip] A norm on a vector space $V$ is 
a function $\|\cdot\|: V \to \mathbb{R}$ which assigns each [[Vector]] vector $x \in V$ its *length* $\|x\| \in \mathbb{R}$.

A norm must satisfy the following properties:
- Absolutely [[Homogeneous]]: $\forall x \in V, \forall \lambda \in \mathbb{R} \quad \|\lambda x\| = |\lambda| \|x\|$
- [[Positive definite]]: $\forall x \in V \quad \|x\| \geq 0$ and $\|x\| = 0 \iff x = 0$
- [[The triangle inequality]] $\forall x, y \in V \quad \|x + y\| \leq \|x\| + \|y\|$


- [[Lp norm]]
	- [[Manhattan norm (L1)]]
	- [[Euclidian norm (L2)]]
	- [[Max norm (L_infinity)]]
- [[Unit vector]]

 




