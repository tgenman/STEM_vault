---
aliases:
  - Обратная матрица
anki: true
created: 2024-04-16 19:39
parent:
  - "[[Matrix]]"
  - "[[Matrix Operations]]"
  - "[[Calculation Matrix Inverse]]"
connected:
  - "[[Matrix Transpose]]"
  - "[[Square matrix]]"
tags: []
---

> [!tip] Matrix Inverse
Consider a [[Square matrix]] $A \in \mathbb{R}^{n \times n}$. Let matrix $B \in \mathbb{R}^{n \times n}$ have the property that $AB = I_n = BA$. $B$ is called the inverse of $A$ and denoted by $A^{-1}$.


### Properties of Matrix Inverse
- ==Matrix Inverse== определяется единственным образом;
- [[Matrix|Матрица]] имеет обратную матрицу, только если [[Determinant of matrix|определитель]] не равен нулю
- Обратные матрицы существуют только для квадратных.
- $AA^{−1}=A^{−1}A=E$
- $(AB)^{−1}=B^{−1}A^{−1}$
-  $(A + B)^{−1} \neq A^{−1} + B^{−1}$
- $(A^{−1})^{−1}=A$
- $(A^{−1})^T=(A^T)^{−1}$
- $(αA)^{−1}=α^{−1}A^{−1}=A^{−1}α^{−1},α\ne 0$

## обратимость и нулевое решение

- форма матрицы для обращения важна, потому что умножение на нее должно работать с обеих сторон и быть одинаковой и равной матрице идентичности
- Из этого следует что если столбцы линейно зависимы, то при умножение на вектор строку из их можно подобрать такой вектор, что получится ноль.
- А из нуля нельзя восстановить. То есть обратить. Потому эта матрица необратная. И потому все столбцы должны быть линейно независимы
- **Note 4** (Important) *Suppose there is a nonzero vector* ${x}$ *such that* ${Ax = 0}$. *Then* ${A}$ *cannot have an inverse.* No matrix can bring 0 back to ${x}$.
- **If** ${A}$ **is invertible, then** ${Ax = 0}$ **can only have the zero solution** ${x = A^{-1}0 = 0}$.

# Anki
TARGET DECK: math::linal
START
math_complex
FRONT: Matrix Inverse
BACK: Consider a square matrix $A \in \mathbb{R}^{n \times n}$. Let matrix $B \in \mathbb{R}^{n \times n}$ have the property that $AB = I_n = BA$. $B$ is called the inverse of $A$ and denoted by $A^{-1}$.
FORMULA:
ADDITIONAL:
PICTURE:
ID: 1713287272971
END

TARGET DECK: math::linal
START
math_complex
FRONT: Properties of Matrix Inverse
BACK:
- ==Matrix Inverse== определяется единственным образом;
- [[Matrix|Матрица]] имеет обратную матрицу, только если [[Determinant of matrix|определитель]] не равен нулю
- Обратные матрицы существуют только для квадратных.
- $AA^{−1}=A^{−1}A=E$
- $(AB)^{−1}=B^{−1}A^{−1}$
-  $(A + B)^{−1} \neq A^{−1} + B^{−1}$
- $(A^{−1})^{−1}=A$
- $(A^{−1})^T=(A^T)^{−1}$
- $(αA)^{−1}=α^{−1}A^{−1}=A^{−1}α^{−1},α\ne 0$
FORMULA:
ADDITIONAL:
PICTURE:
ID: 1713287272977
END
