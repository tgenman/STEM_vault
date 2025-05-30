---
aliases:
  - Транспонирование матрицы
anki: true
created: 2023-10-30 20:14
parent:
  - "[[Matrix Operations]]"
connected:
  - "[[Symmetric matrix]]"
  - "[[Matrix Inverse]]"
tags:
---

> [!tip] Matrix Transpose
For $A \in \mathbb{R}^{m \times n}$ the matrix $B \in \mathbb{R}^{n \times m}$ with $b_{ij} = a_{ji}$ is called the transpose of $A$. We write $B = A^T$.


$$\mathrm{A}=\begin{pmatrix}\color{blue}{a_{11}}&\color{blue}{a_{12}}&\color{blue}{a_{13}}&\ldots&\color{blue}{a_{1n}}\\\color{blue}{a_{21}}&\color{blue}{a_{22}}&\color{blue}{a_{23}}&\ldots&\color{blue}{a_{2n}}\\\ldots&\ldots&\ldots&\ldots&\ldots\\\color{blue}{a_{m1}}&\color{blue}{a_{m2}}&\color{blue}{a_{m3}}&\ldots&\color{blue}{a_{mn}}\end{pmatrix}\quad\mathrm{A}^\mathrm{T}=\begin{pmatrix}\color{blue}{a_{11}}&\color{blue}{a_{21}}&\ldots&\color{blue}{a_{m1}}\\\color{blue}{a_{12}}&\color{blue}{a_{22}}&\ldots&\color{blue}{a_{m2}}\\\color{blue}{a_{13}}&\color{blue}{a_{23}}&\ldots&\color{blue}{a_{m3}}\\\ldots&\ldots&\ldots&\ldots\\\color{blue}{a_{1n}}&\color{blue}{a_{2n}}&\ldots&\color{blue}{a_{mn}}\end{pmatrix}$$


### Properties of Matrix Transpose
-   $(A^{T})^{T}=A$
-   $(A+B)^{T}=A^{T}+B^{T}$
-   $(AB)^{T}=B^{T}A^{T}$
-   $(\lambda A)^{T}=\lambda A^{T}$
-   $\det A=\det A^{T}$
- $(A^{−1})^T=(A^T)^{−1}$


# Anki
TARGET DECK: math::linal
START
math_complex
FRONT: Matrix Transpose
BACK: For $A \in \mathbb{R}^{m \times n}$ the matrix $B \in \mathbb{R}^{n \times m}$ with $b_{ij} = a_{ji}$ is called the transpose of $A$. We write $B = A^T$.
FORMULA: $$\mathrm{A}=\begin{pmatrix}\color{blue}{a_{11}}&\color{blue}{a_{12}}&\color{blue}{a_{13}}&\ldots&\color{blue}{a_{1n}}\\\color{blue}{a_{21}}&\color{blue}{a_{22}}&\color{blue}{a_{23}}&\ldots&\color{blue}{a_{2n}}\\\ldots&\ldots&\ldots&\ldots&\ldots\\\color{blue}{a_{m1}}&\color{blue}{a_{m2}}&\color{blue}{a_{m3}}&\ldots&\color{blue}{a_{mn}}\end{pmatrix}\quad\mathrm{A}^\mathrm{T}=\begin{pmatrix}\color{blue}{a_{11}}&\color{blue}{a_{21}}&\ldots&\color{blue}{a_{m1}}\\\color{blue}{a_{12}}&\color{blue}{a_{22}}&\ldots&\color{blue}{a_{m2}}\\\color{blue}{a_{13}}&\color{blue}{a_{23}}&\ldots&\color{blue}{a_{m3}}\\\ldots&\ldots&\ldots&\ldots\\\color{blue}{a_{1n}}&\color{blue}{a_{2n}}&\ldots&\color{blue}{a_{mn}}\end{pmatrix}$$
ADDITIONAL:
PICTURE:
ID: 1713286369390
END

TARGET DECK: math::linal  
START
math_complex
FRONT: Properties of Matrix Transpose
BACK: 
-   $(A^{T})^{T}=A$
-   $(A+B)^{T}=A^{T}+B^{T}$
-   $(AB)^{T}=B^{T}A^{T}$
-   $(\lambda A)^{T}=\lambda A^{T}$
-   $\det A=\det A^{T}$
- $(A^{−1})^T=(A^T)^{−1}$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1713286421084
END