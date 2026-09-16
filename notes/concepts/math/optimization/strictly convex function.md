---
aliases:
  - Строго выпуклая функция
anki: false
created: "2026-09-15"
parent:
  - "[[519.853.3 Convex optimization MOC]]"
connected:
  - "[[Convex function]]"
  - "[[Strongly Convex Function]]"
tags:
  - контент/определение
---

> [!tip] strictly convex function
> A function $f:C\to\mathbb R$ on a convex set $C$ is strictly convex if, for distinct $x,y\in C$ and $t\in(0,1)$,
> $$f((1-t)x+ty)<(1-t)f(x)+tf(y).$$

[[Strongly Convex Function|Strong convexity]] with a positive constant implies strict convexity. Strict convexity does not require a uniform positive quadratic lower bound.

For example, $f(x)=x^4$ is strictly convex on $\mathbb R$, but not strongly convex there: $f''(0)=0$.

Основа переноса: [[519.853.3 Convex optimization MOC]]. Условия и рассуждения уточнены при разборе; внешняя атрибуция первоисточника не проверена.
