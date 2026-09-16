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
- Even when $A$, $B$ and $A+B$ are invertible, $(A+B)^{-1}=A^{-1}+B^{-1}$ is not a general identity.
- $(A^{−1})^{−1}=A$ 
- $(A^{−1})^T=(A^T)^{−1}$
- $(αA)^{−1}=α^{−1}A^{−1}=A^{−1}α^{−1},α\ne 0$

## обратимость и нулевое решение

For a square matrix $A$, if there is $x\ne0$ with $Ax=0$, then $A$ cannot be invertible: otherwise
$$
x=A^{-1}Ax=A^{-1}0=0,
$$
a contradiction. Equivalently, an invertible matrix has only the zero solution of $Ax=0$. This is the obstruction described in the original map.

Источник переноса: [[512.64  Linear algebra MOC]].

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
- Even when $A$, $B$ and $A+B$ are invertible, $(A+B)^{-1}=A^{-1}+B^{-1}$ is not a general identity.
- $(A^{−1})^{−1}=A$ 
- $(A^{−1})^T=(A^T)^{−1}$
- $(αA)^{−1}=α^{−1}A^{−1}=A^{−1}α^{−1},α\ne 0$ 
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1713287272977
END

