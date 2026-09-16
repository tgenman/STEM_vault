---
aliases:
  - Критерий выпуклости второго порядка
anki: false
created: "2026-09-15"
parent:
  - "[[519.853.3 Convex optimization MOC]]"
connected:
  - "[[Convex function]]"
  - "[[Strongly Convex Function]]"
  - "[[Hessian]]"
tags:
  - контент/теорема
---

> [!tip] second-order criterion
> Let $C\subseteq\mathbb R^n$ be nonempty, open and convex and let $f\in C^2(C)$. For $m\ge0$,
> $$\nabla^2 f(x)\succeq mI\quad\text{for every }x\in C$$
> characterizes convexity for $m=0$, and $m$-strong convexity for $m>0$.

## proof

Set $g(x)=f(x)-m\|x\|_2^2/2$. Along a segment with direction $v$, the second derivative of the restriction of $g$ is
$v^\top(\nabla^2 f(x)-mI)v$.
Nonnegativity in every direction is equivalent to convexity of every line restriction, hence to convexity of $g$.

Positive definiteness at each point without a common positive lower bound is not the strong-convexity condition stated here.

Основа переноса: [[519.853.3 Convex optimization MOC]]. Условия и рассуждения уточнены при разборе; внешняя атрибуция первоисточника не проверена.
