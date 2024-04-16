---
aliases:
  - Умножение матрицы на матрицу
tags: 
publish: true
created: 2024-04-16 19:17
parent:
  - "[[Matrix]]"
connected:
  - "[[Commutative matrix]]"
---

Матрицу $A$ можно умножить на матрицу $B$ только если количество столбцов $A$ равно количеству строк B.B.

$A_{m{\times}n}\cdot B_{n{\times}k}=C_{m{\times}k}$

![[Pasted image 20240416191844.png]]



> Произведение матриц в общем случае некоммутативно.


The product of two matrices is given by:

$$
\left[
\begin{matrix}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33} \\
\end{matrix}
\right]
\cdot
\left[
\begin{matrix}
k_{11} & k_{12} \\
k_{21} & k_{22} \\
k_{31} & k_{32} \\
\end{matrix}
\right]
=
\left[
\begin{matrix}
a_{11} \cdot k_{11} + a_{12} \cdot k_{21} + a_{13} \cdot k_{31} & a_{11} \cdot k_{12} + a_{12} \cdot k_{22} + a_{13} \cdot k_{32} \\
a_{21} \cdot k_{11} + a_{22} \cdot k_{21} + a_{23} \cdot k_{31} & a_{21} \cdot k_{12} + a_{22} \cdot k_{22} + a_{23} \cdot k_{32} \\
a_{31} \cdot k_{11} + a_{32} \cdot k_{21} + a_{33} \cdot k_{31} & a_{31} \cdot k_{12} + a_{32} \cdot k_{22} + a_{33} \cdot k_{32} \\
\end{matrix}
\right]
$$


