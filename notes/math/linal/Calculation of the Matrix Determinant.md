---
aliases:
  - Вычисление определителя матрицы
publish: true
created: 2023-10-30 20:33
parent:
  - "[[Determinant of matrix|Определитель матрицы]]"
connected: 
tags:
  - anki
---
## 1х1
$$|(a_{11})| = a_{11}$$

## 2х2
![[Pasted image 20220725164200.png|500]]


$$\begin{vmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{vmatrix}=a_{11}\cdot a_{22}-a_{12}\cdot a_{21}$$
Определитель матрицы BB получился отрицательным, её векторы образуют левую пару. Сделаем вывод:

Если ориентация системы векторов изменилась, то и определитель поменял знак.

## 3x3 
### Правило Саррюса  [[👤 Sarrus, Pierre-Frederic]]
![[Pasted image 20220725181532.png]]

### Правило разложения [[Determinant of matrix|определителя]] 

**Минор** — это [[Determinant of matrix|определитель матрицы]]  $B_{m{\times}m}$, которая получена из матрицы $A_{n{\times}n}$ путём удаления одной или нескольких её строк и столбцов.

**Дополнительный минор** $M_{ij}$ элемента $a_{ij}$ матрицы $A_{n{\times}n}$ — это [[Determinant of matrix|определитель матрицы]] , полученной из матрицы $A_{n{\times}n}$ вычёркиванием $ii$-той строки и $jj$-того столбца.

**Алгебраическим дополнением** $A_{ij}$ к элементу $a_{ij}$ матрицы $A_{n{\times}n}$ называют число

$$A_{ij}=(-1)^{i+j}\cdot M_{ij}$$

где $M_{ij}$ — дополнительный минор элемента $a_{ij}$.

Прелесть алгебраического дополнения в том, что его знак не зависит от конкретных элементов матрицы. Сумма номеров чётная — будет плюс, нечётная — будет минус.

$$\begin{pmatrix}+&-&+\\-&+&-\\+&-&+\end{pmatrix}$$


$$∣A∣=a_{11}A_{11}+a_{12}A_{12}+a_{13}A_{13}$$

$$\begin{aligned}
&\left.\det A=a_{11}\cdot\left|\begin{array}{cc}\color{red}{a_{22}}&\color{red}{a_{23}}\\\\\color{red}{a_{32}}&\color{red}{a_{33}}\end{array}\right.\right|-a_{12}\cdot\left|\begin{array}{rr}\color{red}{a_{21}}&\color{red}{a_{23}}\\\\\color{red}{a_{31}}&\color{red}{a_{33}}\end{array}\right|+a_{13}\cdot\left|\begin{array}{rr}\color{red}{a_{21}}&\color{red}{a_{23}}\\\\\color{red}{a_{31}}&\color{red}{a_{32}}\end{array}\right|= \\
&=a_{11}\cdot(\color{red}{a_{22}\cdot a_{33}-a_{23}\cdot a_{32}})-a_{12}\cdot(\color{red}{a_{21}\cdot a_{33}-a_{23}\cdot a_{31}}) \\
&+a_{13}\cdot\left(\color{red}{a_{21}\cdot a_{32}-a_{22}\cdot a_{31}}\right)
\end{aligned}$$


Любую квадратную матрицу $A_{n{\times}n}$ можно разложить по **любой** строке или столбцу.


$$|A|=\displaystyle\sum_{i=1}^n a_{iq}A_{iq}=\displaystyle\sum_{j=1}^n a_{pj}A_{pj}$$

где $p{,}\ {q}$ — номера произвольной строки и столбца матрицы $A$.