---
aliases:
  - Векторное произведение векторов
created: 2024-07-03 22:11
parent: 
connected:
  - "#обс/linking"
tags:
  - fix/empty
---


это просто [[Determinant of matrix|Детерминант матрицы]] взятый с ориентацией

$\vec{a} = a_x \vec{i} + a_y \vec{j} + a_z \vec{k}$  
$\vec{b} = b_x \vec{i} + b_y \vec{j} + b_z \vec{k}$ 

$$
\vec{a} \times \vec{b} = 
\begin{bmatrix}
a_x \\ a_y \\ a_z
\end{bmatrix} \times
\begin{bmatrix}
b_x \\ b_y \\ b_z
\end{bmatrix} = \det(
\begin{bmatrix}
\vec{i} & a_x & b_x \\ \vec{j} & a_y & b_y \\ \vec{k} & a_z & b_z
\end{bmatrix} )
= (a_y b_z - a_z b_y) \vec{i} + (a_z b_x - a_x b_z) \vec{j} + (a_x b_y - a_y b_x) \vec{k}
$$

$$
||\vec{a} \times \vec{b}|| = ||\vec{a}|| ||\vec{b}|| \sin{\phi}
$$

![[Pasted image 20230909183544.png|300]]

$[\bar a \times \bar b ]$
$[\bar a \times \bar b ] = - [\bar b \times \bar a ]$
$[\bar a \times \bar a] = 0$

![[Pasted image 20230812185525.png|300]]

==Векторным произведением== $[\bar a \times \bar b ]$  [[Collinear vectors|неколлинеарных векторов]]  $\bar a$ и $\bar b$ , взятых в данном порядке, называется ВЕКТОР $\bar N$ , длина которого численно равна площади параллелограмма, построенного на данных векторах; 

Вектор $\bar N$  [[Orthogonal vectors|ортогонален]] векторам $\bar a$ и $\bar b$ ,  и направлен так, что [[Basis VS|базис]] $(\bar a; \bar b; \bar N)$ имеет правую ориентацию [[Правые и левые упорядоченные тройки]]] .




**Connected with:**
- [[Vectors opeartions]]
- [[Inner product]]

