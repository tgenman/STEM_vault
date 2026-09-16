---
aliases:
  - Критерий выпуклости первого порядка
anki: false
created: "2026-09-15"
parent:
  - "[[519.853.3 Convex optimization MOC]]"
connected:
  - "[[Convex function]]"
  - "[[Strongly Convex Function]]"
  - "[[Gradient]]"
tags:
  - контент/теорема
---

### Theorem (First-order criterion)
Let a function $f(x)$ be differentiable and its domain be a convex set $\mathcal{X} \subseteq \mathbb{R}^n$. Then $f(x)$ is strongly convex with $m \geq 0$ if and only if:
$$f(x) - f(x^*) \geq \langle f'(x^*), x - x^* \rangle + \frac{m}{2} \|x - x^*\|_2^2, \quad \forall x, x^* \in \mathcal{X}.$$


![[Pasted image 20241017233914.png|400]]
