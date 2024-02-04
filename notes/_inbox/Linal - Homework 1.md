## Topics covered: matrices, algebra preliminaries.
Throughout, $Mat_{m \times n}(K)$ denotes the set of $m$ by $n$ matrices over a field $K^{[1]}$; a matrix $A \in Mat_{m \times n}(K)$ is a rectangular table $[a_{ij}]$ with $m$ rows and $n$ columns whose entries are elements $a_{ij}$ ($i$ is the row index, $j$ is the column index) of the base field $K$.

Given two matrices $A \in Mat_{m \times n}(K)$ and $B \in Mat_{n \times p}(K)$, their product $AB$ is an element of $Mat_{m \times p}(K)$. Entry-wise we have $(AB) = [c_{ij}], c_{ij} = \sum_{k=1}^{n} a_{ik}b_{kj}$. For **square matrices** ($A \in Mat_{n \times n}(K)$), the matrix product is a binary operation that, together with entry-wise addition and multiplication by scalars from $K$, turns $Mat_{n \times n}(K)$ into an associative unital $K$-algebra of dimension $n^2$.

The set $GL_n(K) \subset Mat_{n \times n}(K)$ of all invertible (w.r.t. matrix multiplication) square $n$ by $n$ matrices is a group under the matrix multiplication.

For fixed $i$ and $j$, the matrix $E_{ij}$ is the matrix with $1$ in the $(i,j)$-entry and zero elsewhere.

### 1.1. (A few direct computation examples)
A. Compute the following matrix products:

$$
A = \left[ \begin{array}{cc}
\cos \alpha & -\sin \alpha \\
\sin \alpha & \cos \alpha \\
\end{array} \right]^n,
$$
$$
B = \left[ \begin{array}{c}
\lambda \\
0 \\
\end{array} \right]^n,
$$
$$
C = \left[ \begin{array}{cc}
2 & 1 \\
5 & 3 \\
\end{array} \right]
\cdot
\left[ \begin{array}{cc}
0 & -1 \\
1 & -5 \\
\end{array} \right]^n
$$

B. Given a square matrix $A$ and a polynomial $f(t) = a_0 + a_1t + \ldots + a_kt^k$ in one variable (both over $K$), the notation $f(A)$ stands for the matrix $f(A) = a_0I + a_1A + \ldots + a_kA^k$ (I is the identity matrix of the same size as $A$). Suppose $A$ and $C$ are square matrices of the same size and $C$ is invertible. Prove that $f(CAC^{-1}) = Cf(A)C^{-1}$.

### 1.2. (Some basic algebra)
A. Let $A$ be a matrix. Find the matrix $E_{ij}A$.

B. Let $A$ be a matrix. Find the matrix $AE_{ij}$.

C. Let $A$ be a square matrix such that for all $i, j$ one has $E_{ij}A = AE_{ij}$. Prove that $A$ is a scalar matrix, i.e. $A = \lambda I$ (I is the identity matrix) for some $\lambda \in K$.

D. Recall that for a group $G$, its center $Z(G)$ is the set of all $h \in G$ such that $h$ commutes with every element $g \in G$: $gh = hg$. What is the center of $GL_n(K)$?

E. Let $A$ be a square matrix such that for all $i$ one has $E_{ii}A = AE_{ii}$. Prove that $A$ is a diagonal matrix.





Давайте сформулируем и докажем процесс умножения матрицы $E_{ij}$ на матрицу $A \in Mat_{m \times n}(K)$ более формально, используя математическую нотацию. Мы хотим показать, что результатом умножения будет матрица, где все элементы равны $0$, за исключением элементов в $i$-й строке, которые соответствуют элементам $j$-го столбца матрицы $A$, расположенными в строке.

### Предположения

- $E_{ij}$ — матрица размера $m \times n$, где все элементы равны $0$, кроме элемента в позиции $(i, j)$, который равен $1$.
- $A$ — матрица размера $m \times n$ над полем $K$ с элементами $a_{pq}$, где $p$ обозначает номер строки, а $q$ — номер столбца.
- Мы хотим найти матрицу $C = E_{ij}A$.

### Доказательство

Пусть $C = E_{ij}A$. Элементы матрицы $C$ обозначим как $c_{pq}$. Тогда по определению умножения матриц:

$c_{pq} = \sum_{k=1}^{n} e_{pk}a_{kq}$

Так как в матрице $E_{ij}$ все элементы равны $0$, кроме $e_{ij} = 1$, данное уравнение упрощается до:

1. Если $p \neq i$, то для любого $k$ $e_{pk} = 0$, следовательно, $c_{pq} = 0$ для всех $q$, так как нет соответствующего ненулевого элемента $e_{pk}$, который мог бы участвовать в суммировании.
2. Если $p = i$, то уравнение упрощается до $c_{iq} = e_{ik}a_{kq}$. В данном случае, единственный ненулевой элемент $e_{ik}$ — это $e_{ij}$, следовательно, $c_{iq} = a_{jq}$ для всех $q$.

Таким образом, мы получаем, что $c_{pq} = 0$ для всех $p \neq i$, а для $p = i$, $c_{iq} = a_{jq}$, что означает, что $i$-я строка матрицы $C$ является копией $j$-го столбца матрицы $A$, расположенной в строке, а все остальные элементы равны $0$.

### Заключение

Этот результат демонстрирует, как действие матрицы $E_{ij}$ на матрицу $A$ выделяет $j$-й столбец из $A$ и помещает его в $i$-ю строку результирующей матрицы, оставляя все другие элементы равными нулю. Это простое, но мощное свойство матриц $E_{ij}$ играет ключевую роль в теории матриц и их применениях, например, в преобразованиях линейных пространств.