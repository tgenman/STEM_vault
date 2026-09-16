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

> [!tip] local minimum is global
> If $C\subseteq\mathbb R^n$ is convex and $f:C\to\mathbb R$ is convex, every local minimum relative to $C$ is a global minimum on $C$.

## proof

Let $x^*$ be a local minimum. If it is not global, there is a feasible point $y$ with $f(y)<f(x^*)$; no assumption that a global minimum is attained is needed.

Choose $t\in(0,1)$ small enough that $z=(1-t)x^*+ty$ lies in the neighbourhood of local minimality. Convexity of $C$ gives $z\in C$, and
$$
f(z)\le(1-t)f(x^*)+tf(y)<f(x^*),
$$
a contradiction.

Основа переноса: [[519.853.3 Convex optimization MOC]]. Условия и рассуждения уточнены при разборе; внешняя атрибуция первоисточника не проверена.
