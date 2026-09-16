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

> [!tip] first-order criterion
> Let $C\subseteq\mathbb R^n$ be nonempty, open and convex, let $f:C\to\mathbb R$ be differentiable, and fix $m\ge0$. Then
> $$f(y)\ge f(x)+\langle\nabla f(x),y-x\rangle+\frac m2\|y-x\|_2^2,\qquad x,y\in C,$$
> is equivalent to convexity when $m=0$, and to $m$-strong convexity when $m>0$.

## proof

For $m=0$, convexity gives
$f(x+t(y-x))\le(1-t)f(x)+tf(y)$. Divide by $t>0$ and let $t\downarrow0$ to obtain the lower bound.

Conversely, apply the lower bound at $z=(1-t)x+ty$ to $x$ and $y$, then take the weighted sum: the gradient terms cancel and yield convexity.

For general $m$, apply the $m=0$ result to $g(x)=f(x)-m\|x\|_2^2/2$, expanding the quadratic term.

![[Pasted image 20241017233914.png|400]]

Основа переноса: [[519.853.3 Convex optimization MOC]]. Условия и рассуждения уточнены при разборе; внешняя атрибуция первоисточника не проверена.
