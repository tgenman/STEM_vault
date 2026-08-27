---
aliases:
  - Вершинная связность k(G)
  - Connectivity k(G)
anki: false
created: 2024-09-13 18:48
parent:
  - "[[519.173.5 Числовые характеристики графов]]"
connected:
  - "[[Edge-connectivity lambda(G)]]"
tags:
  - fix/empty
---

> [!tip] Vertex-connectivity k(G)
minimum size of [[Vertex-cut]]

Если удалить все вершины и ребра, с которыми связаны вершины множества $W$, то граф перестанет быть связным
$$\kappa(G) = \varkappa(G) := \min\{k:\exists W\subseteq V\}$$
Это число $\varkappa$ называется вершинной связностью.

- $0 <= k(G) <= |G| - 1$
- $k(K_{n}) = n-1$