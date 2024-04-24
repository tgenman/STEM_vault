---
aliases:
  - Нахождение обратной матрицы
publish: true
anki: false
created: 2024-04-16 20:05
parent:
  - "[[Matrix Inverse]]"
connected:
  - "[[Matrix Operations]]"
tags: []
---


$$A^{-1}=\dfrac1{|A|}\cdot {A_{ij}}^T,$$
где $|A|$ — определитель матрицы $A$,

${A_{ij}}^T$ — транспонированная матрица алгебраических дополнений соответствующих элементов матрицы $A$.

### 2х2
Из исходной матрицы $2{\times}2$ всегда получают транспонированную матрицу алгебраических дополнений одним и тем же образом: элементы главной диагонали меняются местами, элементы побочной меняют знак.

$$\begin{pmatrix} a & b \\ c & d \end{pmatrix}^{-1} = \dfrac{1}{a d - bc} \begin{pmatrix} d & -b \\ -c & a \end{pmatrix}$$

### Способы нахождения
- Adjugate 
- Using row operations
- Using [[Elementary transformations]]


---

Чтобы подчеркнуть, что было до преобразования, а что получилось после, 
точку $W$ называют **образом** точки $Z$, а 
точку $Z$ — **прообразом** точки $W$  - до умножения на [[Матрица линейного преобразования]]


