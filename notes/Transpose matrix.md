---
aliases:
  - Транспонирование матрицы
publish: true
anki: false
created: 2023-10-30 20:14
parent:
  - "[[Matrix|Матрица]]"
connected:
  - "[[Симметричная матрица]]"
---
В матрицах можно не только менять местами столбцы или строки, но и превращать строки в столбцы.

> [!Определение]
> **Транспонировать** матрицу $A=(a_{ij})_{m{\times}n}$ значит, записать её строки в столбцы с сохранением порядка следования. В результате получается матрица
$A^{T}=(a_{ji})_{n{\times}m}$

Транспонированную матрицу помечают надстрочным индексом $^{T}$.

$$\mathrm{A}=\begin{pmatrix}\color{blue}{a_{11}}&\color{blue}{a_{12}}&\color{blue}{a_{13}}&\ldots&\color{blue}{a_{1n}}\\\color{blue}{a_{21}}&\color{blue}{a_{22}}&\color{blue}{a_{23}}&\ldots&\color{blue}{a_{2n}}\\\ldots&\ldots&\ldots&\ldots&\ldots\\\color{blue}{a_{m1}}&\color{blue}{a_{m2}}&\color{blue}{a_{m3}}&\ldots&\color{blue}{a_{mn}}\end{pmatrix}\quad\mathrm{A}^\mathrm{T}=\begin{pmatrix}\color{blue}{a_{11}}&\color{blue}{a_{21}}&\ldots&\color{blue}{a_{m1}}\\\color{blue}{a_{12}}&\color{blue}{a_{22}}&\ldots&\color{blue}{a_{m2}}\\\color{blue}{a_{13}}&\color{blue}{a_{23}}&\ldots&\color{blue}{a_{m3}}\\\ldots&\ldots&\ldots&\ldots\\\color{blue}{a_{1n}}&\color{blue}{a_{2n}}&\ldots&\color{blue}{a_{mn}}\end{pmatrix}$$

### Свойства транспонированных матриц
-   Дважды транспонированная матрица А равна исходной матрице А.

$(A^{T})^{T}=A$

-   Транспонированная сумма матриц равна сумме транспонированных матриц.

$(A+B)^{T}=A^{T}+B^{T}$

-   Транспонированное произведение матриц равно произведению транспонированных матриц, взятых в обратном порядке.

$(AB)^{T}=B^{T}A^{T}$

-   При транспонировании можно выносить скаляр.

$(\lambda A)^{T}=\lambda A^{T}$

-   [[Determinant of matrix|Определитель]] транспонированной матрицы равен определителю исходной матрицы.

$\det A=\det A^{T}$