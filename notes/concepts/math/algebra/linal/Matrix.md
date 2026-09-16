---
aliases:
  - Матрица
parent: "[[Linear algebra (field)]]"
---
==Матрицей== размера $𝑚 × 𝑛$ называется упорядоченная прямоугольная таблица чисел, имеющая $𝑚$ строк и $𝑛$ столбцов.

$$A=\begin{pmatrix} a_{11} & a_{12} & a_{13} & ... & a_{1n} \\ a_{21} & a_{22} & a_{23} & ... & a_{2n} \\ a_{31} & a_{32} & a_{33} & ... & a_{3n} \\ ... & ... & ... & ... & ... \\ a_{m1} & a_{m2} & a_{m3} & ... & a_{mn} \end{pmatrix}=(a_{ij})_{m{\times}n}$$



В **прямоугольной** матрице количество строк не совпадает с количеством столбцов. 
В [[Square matrix|квадратной]]  количество строк и столбцов совпадает. 



> [!Равные матрицы]
> Если две матрицы $A=(a_{ij})_{m{\times}n}$ и $B=(b_{ij})_{m{\times}n}$ одного размера и совпадают поэлементно, то эти матрицы **равны**.

> [!Эквивалентные матрицы]
> Матрицы называют **эквивалентными**, если одну из другой можно получить перестановкой строк или столбцов. При этом матрицы не являются равными.



### **Свойства сложения**
Для произвольных матриц $A=(a_{ij})_{m{\times}n}{,}\ B=(b_{ij})_{m{\times}n}{,}\ C=(c_{ij})_{m{\times}n}$ одинакового размера $m{\times}n$ действуют свойства:
1) $A+B=B+A$  — коммутативность;
2) $(A+B)+ C=A+ (B+C)$  — ассоциативность;
3) \ $A+O=A$ — прибавление нулевой матрицы;
4) \ $\forall\ A\ \exists!\ B{:}\ \ A+B=O$ — для любой матрицы существует единственная, противоположная ей.
5) \ $(A+B)^{T}=A^{T}+B^{T}$ — транспонированная сумма матриц равна сумме этих транспонированных матриц.

### Свойства умножения на скаляр
1) $1\cdot A=A$; 
2) $-1\cdot A=-A$.
3) $0\cdot A= \begin{pmatrix} 0 & 0 & 0 & … & 0 \\ 0 & 0 & 0 & … & 0 \\ 0 & 0 & 0 & … & 0 \\ \cdots & \cdots & \cdots & \cdots & \cdots \\ 0 & 0 & 0 & … & 0 \end{pmatrix}$
4) Для любого числа $k\in\mathbb{R}$ умножение на скаляр коммутативно: $k\cdot A=A\cdot k$.
5) Для любых чисел $k{,}\ m\in \mathbb{R}$ можно сначала найти произведение скаляров, а потом умножать на матрицу: $k\cdot(m\cdot A)=(k\cdot m)\cdot A$.
6) $(k\cdot A)^{T}=k\cdot A^{T}$ — можно сначала транспонировать исходную матрицу и после этого умножать на скаляр.

### Свойста перемножения матриц
1) $\ AB\neq BA$ - некоммутативность (если они не перестановочные)
2) $\ A(BC)=(AB)C$  - ассоциатичность
3) \ $AE=EA=A$. - умножение на единичную матрицу
4) Дистрибутивность относительно сложения:
        $(A+B)\cdot C= AC+BC$;
        $K(A+B)=KA+KB$.
5) $(\alpha A B)=\alpha(AB)=A(\alpha B)$. - Ассоциативность умножения на скаляр
6) Транспонирование произведения:
        $(AB)^T=B^T\cdot A^T$;
        $(kA)^T=A^T\cdot k ^T$;
        $(Am)^T=m^T\cdot A^T$.

![[Matrix Inverse#Properties of Matrix Inverse]]

## алгебраическая структура

For a field $F$ and fixed positive dimensions $m,n$, $M_{m,n}(F)$ is a [[Linear (vector) space|vector space]] under [[Matrix Addition]] and [[Matrix Scalar Multiplication]]. Its additive structure is an [[Abelian group]]: the [[Identity element|identity]] is [[Zero Matrix]], and the [[Inverse element|additive inverse]] of $A$ is $-A$.

For square matrices $M_n(F)$:
- [[Matrix Matrix Multiplication]] is associative and has identity [[Identity matrix]], forming a [[Monoid]].
- Addition and multiplication give a unital associative [[Ring (R,+,*)|ring]] and an associative algebra over $F$.
- The invertible matrices form [[general linear group]], not the entire set $M_n(F)$.

[[Matrix Transpose]] maps $M_{m,n}(F)$ to $M_{n,m}(F)$; inversion is defined only on invertible square matrices.

Источник переноса: [[512.64  Linear algebra MOC]].
