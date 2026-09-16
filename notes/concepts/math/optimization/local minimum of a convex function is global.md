---
aliases:
  - Локальный минимум выпуклой функции является глобальным
anki: false
created: "2026-09-15"
parent:
  - "[[519.853.3 Convex optimization MOC]]"
connected:
  - "[[Convex function]]"
  - "[[Convex Set]]"
tags:
  - контент/теорема
---

### Theorem
If $f$ is a convex function and $x^*$ is a point of local minimum, then $x^*$ is a point of global minimum.

### Proof
- Assume that there exists a point $y^*$ such that $y^* \neq x^*$ and $y^*$ is a point of global minimum: $f(y^*) < f(x^*)$.
- By the definition of a point of local minimum: $f(x^*) \leq f(x)$, where $\|x^* - x\|_2 \leq \delta$.
- Choose sufficiently small $\alpha \in (0, 1)$ and consider a point $z = (1-\alpha) x^* + \alpha y^*$ such that $\|x^* - z\|_2 \leq \delta$.
- $$f(x^*) \leq f(z) \leq \alpha f(y^*) + (1-\alpha) f(x^*) < f(x^*).$$
- We get a contradiction, therefore the assumption is incorrect and $x^*$ is a point of global minimum.
