---
aliases: 
created: 2024-07-03 22:14
parent:
  - "[[Matrix Operations]]"
  - "[[Vectors opeartions|Операции над векторами]]"
connected:
  - "[[Vector|Вектор]]"
  - "[[Matrix|Матрица]]"
  - "#обс/linking"
tags:
  - fix/empty
anki: false
---
Умножение вектора на матрицу даёт новый вектор. Он состоит из скалярных произведений этого вектора со столбцами матрицы.
$$k_{1\times m}\cdot M_{m\times\color{red}{n}}=(k\cdot M)_{\color{red}{1\times n}}.$$


Для скалярного произведения
$$\vec{a}\cdot\vec{b}=a^T\cdot b$$
We can simplify the matrix operation by distributing the scalars across the respective matrices, which yields:

$$\begin{pmatrix}4\cdot0\\2\cdot0\end{pmatrix}+\begin{pmatrix}-6\cdot(-6)\\10\cdot(-6)\end{pmatrix}+\begin{pmatrix}5\cdot4\\-1\cdot4\end{pmatrix}=\begin{pmatrix}4\\2\end{pmatrix}\cdot0+\begin{pmatrix}-6\\10\end{pmatrix}\cdot(-6)+\begin{pmatrix}5\\-1\end{pmatrix}\cdot4.$$



