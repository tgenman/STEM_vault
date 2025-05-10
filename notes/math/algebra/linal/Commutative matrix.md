---
aliases:
  - Перестановочные матрицы
anki: false
connected:
  - "[[Commutative identity]]"
---

> [!tip] [[Commutative identity]] matrix
[[Matrix|Матрицы]], для которых $AB=BA$

Перестановочными бывают только [[Square matrix|квадратные матрицы]]   одного и того же размера.

Например, $A=\begin{pmatrix} 2 & -3 \\ 1 & 0 \end{pmatrix}$ и $B=\begin{pmatrix} 4 & -3 \\ 1 & 2 \end{pmatrix}$. 

$AB=\begin{pmatrix} 2 & -3 \\ 1 & 0 \end{pmatrix}\cdot\begin{pmatrix} 4 & -3 \\ 1 & 2 \end{pmatrix}=\begin{pmatrix}2\cdot4-3\cdot1 & 2\cdot(-3)-3\cdot2 \\ 1\cdot4+0\cdot1 & 1\cdot(-3)+0\cdot2\end{pmatrix}=\begin{pmatrix} 5 & -12 \\ 4 & -3 \end{pmatrix}$.

$BA=\begin{pmatrix} 4 & -3 \\ 1 & 2 \end{pmatrix} \cdot\begin{pmatrix} 2 & -3 \\ 1 & 0 \end{pmatrix}=\begin{pmatrix} 4\cdot2-3\cdot1 & 4\cdot(-3)-3\cdot0 \\ 1\cdot2+2\cdot1 & 1\cdot(-3)+2\cdot0 \end{pmatrix} =\begin{pmatrix} 5 & -12 \\ 4 & -3\end{pmatrix}$

$BA=AB$.

Матрица $B$ — не единственная перестановочная для $A$. Для каждой квадратной матрицы существует бесконечное количество таких «партнёров по коммутативности».

---

[[Zero Matrix]] соответствующего размера будет перестановочной с любой [[Square matrix|квадратной]].

Например, $\begin{pmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{pmatrix}\cdot\begin{pmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{pmatrix}=\begin{pmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9\end{pmatrix}\cdot\begin{pmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{pmatrix}=\begin{pmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{pmatrix}$.

---

То же самое касается и [[Identity matrix|единичной матрицы]]  — она тоже перестановочная со всеми квадратными соответствующего порядка.

