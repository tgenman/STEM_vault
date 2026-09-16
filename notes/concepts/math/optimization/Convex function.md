---
aliases:
  - Выпуклая функция
anki: false
created: 2024-10-27 22:20
parent:
  - "[[Function (math)]]"
  - "[[Convex Set]]"
connected:
  - "[[Concave function]]"
tags:
---

> [!tip] convex function
> A function $f:C\to\mathbb R$ on a convex set $C$ is convex if, for all $x,y\in C$ and $t\in[0,1]$,
> $f((1-t)x+ty)\le(1-t)f(x)+tf(y).$

For the distinct-point strict inequality, see [[strictly convex function]]. For a positive uniform quadratic bound, see [[Strongly Convex Function]].

##### Examples of convex functions
- $x^p$ for $x \geq 0$ and $p \geq 1$
- $x \log x$, where $x > 0$
- $\max\{x_1, \dots, x_n\}$
- $\|\mathbf{x}\|$
- $\log \left( \sum_{i=1}^n e^{x_i} \right)$
- $-\log \det \mathbf{X}$ for $\mathbf{X} \in S_{++}^n$

## критерии и свойства

- [[first-order criterion of convexity]]
- [[second-order criterion of convexity]]
- [[local minimum of a convex function is global]]
- [[operations preserving convexity of functions]]
- [[Jensen Inequality]]

## иллюстрации из карты

![[Convex_supergraph.svg]]
Выпуклая вниз функция, её график выделен синим, и [надграфик](https://ru.wikipedia.org/wiki/%D0%9D%D0%B0%D0%B4%D0%B3%D1%80%D0%B0%D1%84%D0%B8%D0%BA "Надграфик") закрашен зелёным.

![[ConvexFunction.svg]]

Источник переноса: [[519.853.3 Convex optimization MOC]].
