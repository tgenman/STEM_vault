author: **Dmitrii Bondarev** (Дмитрий Бондарев)
group: М05-321сс (**Contemporary Combinatorics**)
date: 2024-02-10
### 4.1. Determinan antidiagonal matrix
Find the formula for the determinant of the matrix $A = [a_{ij}]$ with $a_{ij} = 0$ for $i < n - j + 1$ (i.e. the matrix $A$ has zeros above the antidiagonal).

Since all the elements of the first row, except for the last one ($a_{1n}$), are zero, the expansion of the determinant of $A$ along the first row includes only one non-zero element. Thus, the determinant of $A$ is equal to $a_{1n}$ times the determinant of the submatrix $A'$ of size $(n-1) \times (n-1)$, obtained by removing the first row and the last column from $A$. The submatrix $A'$ also has zeros above its anti-diagonal.
$\text{det}(A) = a_{1n} \cdot \text{det}(A')$

Applying this reasoning recursively to the matrix $A'$ and its subsequent submatrices, we obtain:
$\text{det}(A) = a_{1n} \cdot a_{2, n-1} \cdot \ldots \cdot a_{n1} = \prod_{i=1}^{n} a_{i, n-i+1}.$

### 4.2. 
Compute the determinant of the $n \times n$ matrices $F_{n+1}, n \geq 2$, which are defined as being tridiagonal, with ones on the main diagonal, ones on the diagonal below the main one, and minus ones on the diagonal above the main one. The three matrices following the one-by-one matrix $F_2 = [1]$ in the sequence have the form:
$F_3 = \begin{bmatrix} 1 & -1 & 0 \\ 1 & 1 & -1 \\ 0 & 1 & 1  \end{bmatrix}, \quad F_4 = \begin{bmatrix} 1 & -1 & 0 & 0 \\1 & 1 & -1 & 0 \\ 0 & 1 & 1 & -1 \\0 & 0 & 1 & 1 \end{bmatrix}, \quad F_5 = \begin{bmatrix} 1 & -1 & 0 & 0 & 0 \\ 1 & 1 & -1 & 0 & 0 \\ 0 & 1 & 1 & -1 & 0 \\ 0 & 0 & 1 & 1 & -1 \\ 0 & 0 & 0 & 1 & 1 \end{bmatrix}.$

[Hint: the letter "F" stands for Fibonacci.]

Let $\text{det}(F_{n+1})$ denote the determinant of the matrix $F_{n+1}$. We begin with the base cases:
1. $\text{det}(F_2) = 1$, since $F_2$ is a $1 \times 1$ matrix with the value $1$.
2. $\text{det}(F_3) = 2$, which can be directly computed for a $2 \times 2$ matrix.

For $n \geq 2$, we expand $\text{det}(F_{n+1})$ along the first row, yielding:
$\text{det}(F_{n+1}) = 1 \cdot \text{det}(F'_n) - (-1) \cdot \text{det}(F''_{n-1})$

where:
- $F'_n$ denotes the submatrix of $F_{n+1}$ obtained by removing the first row and the first column, which is structurally equivalent to the matrix $F_n$.
- $F''_{n-1}$ denotes the submatrix of $F_{n+1}$ obtained by removing the first two rows and the first two columns. This submatrix has ones on its main diagonal and ones on the diagonal below the main one, and minus ones on the diagonal above the main one, starting from the third row and column of $F_{n+1}$, making it structurally identical to $F_{n-1}$.

Considering the signs of elements in $F_{n+1}$, the second term in the expression converts to $-(-1) \cdot \text{det}(F''_{n-1}) = \text{det}(F_{n-1})$ (recalling the sign that arises from the determinant expansion and the sign of the element at position $(1,2)$).

Hence, we have established the recursive formula:
$\text{det}(F_{n+1}) = \text{det}(F_n) + \text{det}(F_{n-1})$

which corresponds to the recursive formula for Fibonacci numbers, starting with $\text{det}(F_2) = 1$ and $\text{det}(F_3) = 2$. Therefore, $\text{det}(F_{n+1})$ equals the $n$-th Fibonacci number for $n \geq 2$.

### 4.3. 
How will the determinant of an $n$ by $n$ matrix $A$ change when:

### 4.3.A. Every entry $a_{ij}$ is replaced by $-a_{ij}$.  
For an $n \times n$ matrix $A$ with elements $a_{ij}$, consider matrix $B$ obtained by replacing each $a_{ij}$ with $-a_{ij}$. The task is to find the relationship between $\text{det}(A)$ and $\text{det}(B)$.

Since $B$ is derived by multiplying each row of matrix $A$ by $-1$, and multiplying a row by $-1$ multiplies the determinant by $-1$, the change in the determinant of the matrix after replacing all elements with their opposites is:
$\text{det}(B) = (-1)^n \cdot \text{det}(A).$

This expression shows that $\text{det}(B)$ equals $\text{det}(A)$ multiplied by $(-1)^n$, which depends on the parity of the matrix dimension $n$.

### 4.3.B. The rows $a_{1j}, a_{2j}, \ldots, a_{nj}$ of $A$ are permuted to $a_{nj}, a_{n-1,j}, \ldots, a_{1j}$.  

Let $A$ be an $n \times n$ matrix and $B$ be the matrix obtained from $A$ by permuting its rows in reverse order. We need to determine the relationship between $\text{det}(A)$ and $\text{det}(B)$.

1. **Permutations**: Swapping two rows of the matrix changes the sign of its determinant, $\text{det}(A) \rightarrow -\text{det}(A)$.
2. **Number of swaps** ($k$) to achieve the reverse order:
   - $k = \frac{n}{2}$ for even $n$,
   - $k = \frac{n-1}{2}$ for odd $n$.

The determinant of matrix $B$ is related to the determinant of matrix $A$ as $\text{det}(B) = (-1)^k \cdot \text{det}(A)$, where $k$ is the number of swaps.

$\text{det}(B) = (-1)^{\left\lfloor\frac{n}{2}\right\rfloor} \cdot \text{det}(A).$

### 4.3.C. The columns $a_{i1}, a_{i2}, \ldots, a_{in}$ are permuted to $a_{i2}, \ldots, a_{in}, a_{i1}$.
For a matrix $A$ of order $n$, consider matrix $B$ obtained by cyclically shifting the columns of $A$ one position to the left. The goal is to determine the relationship between $\text{det}(A)$ and $\text{det}(B)$.

A cyclic shift of columns one position to the left is equivalent to performing $n-1$ column transpositions. Each transposition changes the sign of $\text{det}(A)$.

$\text{det}(B) = (-1)^{n-1} \cdot \text{det}(A)$, reflecting the sign change after $n-1$ transpositions.

### 4.4. Let $n$ be an odd number and let $A$ be a skew-symmetric $n$ by $n$ matrix. Show that $\text{det} A = 0$.

From $A^T = -A$, it follows that $\text{det}(A^T) = \text{det}(-A)$. Using the property of the determinant when multiplying a matrix by a scalar, we have $\text{det}(-A) = (-1)^n\text{det}(A)$. Since $\text{det}(A^T) = \text{det}(A)$ for determinants, $\text{det}(A) = (-1)^n\text{det}(A)$.

For odd $n$, $(-1)^n = -1$, hence $\text{det}(A) = -\text{det}(A)$. This is possible only if $\text{det}(A) = 0$.

Thus, $\text{det}(A) = 0$ for any skew-symmetric matrix $A$ of odd order $n$.

### 4.5. Prove that $\text{det} A$ (A has entries in a field $K$) is irreducible as a polynomial in the $n^2$ variables $a_{11}, a_{12}, \ldots, a_{nn}$.

No solution
