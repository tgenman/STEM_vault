---
aliases:
  - Норма вектора
anki: false
parent:
  - "[[Vector|Вектор]]"
  - "[[Norm]]"
connected:
  - "[[Unit vector]]"
  - "[[Inner product]]"
created: 2024-02-03 17:59
moc:
  - "[[512.64  Linear algebra MOC]]"
---

#### Definition
> [!tip] A norm on a vector space $V$ is 
a function $\|\cdot\|: V \to \mathbb{R}$ which assigns each [[Vector]] vector $x \in V$ its *length* $\|x\| \in \mathbb{R}$.

#### Properties
A norm must satisfy the following properties:
- Absolutely [[Homogeneous 1]]: $\forall x \in V, \forall \lambda \in \mathbb{R} \quad \|\lambda x\| = |\lambda| \|x\|$
- [[Positive definite]]: $\forall x \in V \quad \|x\| \geq 0$ and $\|x\| = 0 \iff x = 0$
- [[The triangle inequality]] $\forall x, y \in V \quad \|x + y\| \leq \|x\| + \|y\|$


#### Types
- [[Lp norm]]
    - [[Manhattan norm (L1)]]
    - [[Euclidian norm (L2)]]
    - [[Max norm (L_infinity)]]
- [[Unit vector]]


#### Connection with Inner product
 Any [[Inner product]] inner product induces a ==norm==:
 $\|x\| := \sqrt{\langle x, x \rangle}$

Example: [[Dot product of vectors]]  induces [[Euclidian norm (L2)]]:
$\sqrt{\langle x, x \rangle} = \sqrt{x_1^2 + x_2^2 + \ldots + x_n^2} = \|x\|_2$

(!) Not every ==norm== is induced by an [[Inner product]] inner product.
Example: [[Manhattan norm (L1)]].





