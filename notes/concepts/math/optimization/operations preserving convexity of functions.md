---
aliases:
  - Операции, сохраняющие выпуклость функций
anki: false
created: "2026-09-15"
parent:
  - "[[519.853.3 Convex optimization MOC]]"
connected:
  - "[[Convex function]]"
  - "[[Concave function]]"
  - "[[Operations preserving convexity]]"
tags:
  - контент/саммари
---

> [!tip] operations preserving convexity of functions
> The following constructions preserve convexity on their stated domains.

- Nonnegative sums: if $f_i$ are convex on a common convex domain and $a_i\ge0$, then $\sum_{i=1}^k a_if_i$ is convex.
- Finite pointwise maxima: $\max_{i=1,\ldots,k}f_i$ is convex when each $f_i$ is convex on a common convex domain.
- Affine precomposition: $f(Ax+b)$ is convex on the preimage of the convex domain of $f$.
- Line restrictions: $g(t)=f(x_0+tv)$ are the preceding construction for a scalar argument.
- Scalar composition, sufficient condition: $h\circ f$ is convex if $f$ is convex and $h$ is convex and nondecreasing on an interval containing the range of $f$.

For the last case, first apply monotonicity to the convexity inequality for $f$, then apply convexity of $h$. These are operations on functions, separate from [[Operations preserving convexity|operations on sets]].

Основа переноса: [[519.853.3 Convex optimization MOC]]. Условия и рассуждения уточнены при разборе; внешняя атрибуция первоисточника не проверена.
