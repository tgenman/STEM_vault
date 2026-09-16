---
aliases:
  - Внешнее произведение векторов (outer product)
anki: false
created: "2026-09-15"
parent:
  - "[[512.64  Linear algebra MOC]]"
connected:
  - "[[Vector]]"
  - "[[Matrix]]"
  - "[[Matrix Matrix Multiplication]]"
tags:
  - контент/определение
---

> [!tip] outer product
> For real column vectors $u\in\mathbb R^m$ and $v\in\mathbb R^n$, their outer product is the matrix
> $$uv^\top\in\mathbb R^{m\times n},\qquad (uv^\top)_{ij}=u_i v_j.$$

Unlike a dot product, the result is a matrix rather than a scalar. This note describes the coordinate outer product; it is not the exterior (wedge) product.

For $u=(1,2)^\top$ and $v=(3,4)^\top$:
$$
uv^\top=\begin{pmatrix}3&4\\6&8\end{pmatrix}.
$$

Основа переноса: [[512.64  Linear algebra MOC]]. Условия и рассуждения уточнены при разборе; внешняя атрибуция первоисточника не проверена.
