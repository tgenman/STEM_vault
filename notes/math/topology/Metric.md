---
aliases:
  - Метрика
  - Distance function
anki: false
created: 2025-09-03 20:15
parent:
  - "[[515.1 Topology]]"
connected:
  - "[[Metric space]]"
  - "[[The triangle inequality]]"
tags:
  - content/definition
---
> [!tip] metric
> A **metric** on a set $X$ is a function $d:X\times X\to[0,\infty)$ such that for all $x,y,z\in X$:
> 1. $d(x,y)=0$ if and only if $x=y$;
> 2. $d(x,y)=d(y,x)$;
> 3. $d(x,z)\le d(x,y)+d(y,z)$.

The pair $(X,d)$ is a [[Metric space|metric space]]. The third condition is [[The triangle inequality|the triangle inequality]].
