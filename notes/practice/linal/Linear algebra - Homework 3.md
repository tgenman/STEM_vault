author: **Dmitrii Bondarev** (Дмитрий Бондарев)
group: М05-321сс (**Contemporary Combinatorics**)
date: 2024-02-09

### 3.1. (Yet another numerical example) 
Let $A$ be the matrix $A = \begin{bmatrix} 0 & 1 & 2 & 1 \\ 0 & -1 & 0 & 1 \\ 0 & 1 & -1 & -2 \end{bmatrix}$

#### 3.1.A. Describe the nullspace $N(A)$ of the matrix $A$.  
We need solve equation $Ax=0$
$A = \begin{bmatrix} 0 & 1 & 2 & 1 \\ 0 & 0 & 2 & 2 \\ 0 & 1 & -1 & -2 \end{bmatrix}$
$A = \begin{bmatrix} 0 & 1 & 2 & 1 \\ 0 & 0 & 2 & 2 \\ 0 & 0 & -3 & -3 \end{bmatrix}$
$A = \begin{bmatrix} 0 & 1 & 2 & 1 \\ 0 & 0 & 1 & 1 \\ 0 & 0 & 1 & 1 \end{bmatrix}$
$A = \begin{bmatrix} 0 & 1 & 2 & 1 \\ 0 & 0 & 1 & 1 \\ 0 & 0 & 0 & 0 \end{bmatrix}$

$x_2 + 2x_3 + x_4 = 0$
$x_3 + x_4 = 0$

$x_3 = -x_4$
$x_2 = x_4$.

Letting $x_4 = t$:
- $x_2 = t$
- $x_3 = -t$
- $x_1$ is a free variable, so let $x_1 = s$ (another parameter).

Thus, the general solution and basis for the null space are:
$x = \begin{bmatrix} x_1 \\ x_2 \\ x_3 \\ x_4 \end{bmatrix} = \begin{bmatrix} s \\ t \\ -t \\ t \end{bmatrix} = s\begin{bmatrix} 1 \\ 0 \\ 0 \\ 0 \end{bmatrix} + t\begin{bmatrix} 0 \\ 1 \\ -1 \\ 1 \end{bmatrix}$

Therefore, the basis for the null space is given by the vectors:
$\begin{bmatrix} 1 \\ 0 \\ 0 \\ 0 \end{bmatrix}, \quad \begin{bmatrix} 0 \\ 1 \\ -1 \\ 1 \end{bmatrix}$

Any vector in the null space can be expressed as a linear combination of these two vectors.

#### 3.1.B. Describe the column space $C(A)$ of $A$
(not just as the space of linear combinations of columns as per the definition, but rather as a subspace of $\mathbb{R}^3$ spanned by an appropriate linearly independent system).  
$\text{rref}(A) = \begin{bmatrix} 0 & 1 & 0 & -1 \\ 0 & 0 & 1 & 1 \\ 0 & 0 & 0 & 0 \end{bmatrix}$
is determined by identifying the leading columns in the RREF, which are the second and third columns. These correspond to the basis of $C(A)$ from the original matrix $A$.

The basis for the column space $C(A)$, and therefore the subspace of $\mathbb{R}^3$ it spans, consists of the vectors from the second and third columns of $A$:
- Second column: $\begin{bmatrix} 1 \\ -1 \\ 1 \end{bmatrix}$
- Third column: $\begin{bmatrix} 2 \\ 0 \\ -1 \end{bmatrix}$

Thus, $C(A)$ is spanned by these two linearly independent vectors. The fourth column of $A$ is linearly dependent on the others, indicating it does not contribute to the independence of the system or expand the span of $C(A)$.

#### 3.1.C. What is the reduced row echelon form $\text{rref}(A)$ of $A$?  
$\text{rref}(A) = \begin{bmatrix} 0 & 1 & 0 & -1 \\ 0 & 0 & 1 & 1 \\ 0 & 0 & 0 & 0 \end{bmatrix}$

#### 3.1.D. What is the reduced row echelon form $\text{rref}(B)$ of $B$?
$B = \begin{bmatrix} A & A \\ A & A \end{bmatrix}$
$\text{rref}(B) = \begin{bmatrix} A & A \\ 0 & 0 \end{bmatrix}$


### 3.2. Find the number of $k$-dimensional subspaces in an $n$-dimensional vector space $V$
Let $K = \mathbb{F}_q$ be a finite field with $q$ elements. Find the number of $k$-dimensional subspaces in a vector space $V$ of dimension $n$ over $K^{[1]}$.
[1]: This number is customarily denoted by $\binom{n}{k}$, and is referred to as the Gaussian binomial coefficient.

To find the number of $k$-dimensional subspaces in an $n$-dimensional vector space $V$ over a finite field $\mathbb{F}_q$, we use the Gaussian binomial coefficient, denoted and calculated as follows:
$$\binom{n}{k}_q = \frac{(q^n - 1)(q^n - q) \cdots (q^n - q^{k-1})}{(q^k - 1)(q^k - q) \cdots (q^k - q^{k-1})}.$$

**The numerator** represents the sequence of choices for picking a linearly independent vector, starting with $q^n - 1$ and decreasing each time by a factor of $q$, down to $q^{n-k+1} - 1$. This reflects the number of ways to choose the first, second, up to the $k$-th vector, ensuring each choice is linearly independent from the previous.

**The denominator** similarly represents the ways to select $k$ linearly independent vectors within a $k$-dimensional space, normalizing the result since the order of selection doesn't affect subspace definition.

### 3.3. 
Let $A$ and $B$ be matrices over a field $K$ of size $m \times n$ and $m \times k$, respectively. Show that the matrix equation $AX = B$ where the unknown matrix $X$ has size $n \times k$ has a solution if and only if the rank of the matrix $A$ coincides with the rank of the augmented matrix $[A|B]$

To prove the statement that the matrix equation $AX = B$, where the unknown matrix $X$ has size $n \times k$, has a solution if and only if the rank of matrix $A$ is equal to the rank of the augmented matrix $[A|B]$, we proceed as follows:

**Necessity:** Assume the equation $AX = B$ has a solution. This implies there exists a matrix $X$ such that $AX = B$ holds.

Since each column of $B$ is a linear combination of columns of $A$, the linear span of the columns of $A$ encompasses the columns of $B$. Thus, the rank of $A$ is equal to the rank of the augmented matrix $[A|B]$.

**Sufficiency:** Now, assume the rank of $A$ equals the rank of $[A|B]$.

This equality indicates that the columns of $B$ do not extend the linear span of the columns of $A$, meaning each column of $B$ can be expressed as a linear combination of the columns of $A$.

The existence of matrix $X$, such that $AX = B$, follows from the fact that we can express each column of $B$ through a linear combination of columns of $A$. Consequently, for each column $b_i$ in $B$, there exists a set of coefficients (elements of the corresponding column $x_i$ in $X$) such that $Ax_i = b_i$.

### 3.4.  Write down all known relations between $r, m, n$ in the following cases
Let $A \in \text{Mat}_{m \times n}(\mathbb{R})$ and let $Ax = b$ be a linear system. Denote by $r$ the rank of $A$.

### 3.4.A. $Ax = b$ has no solution for some $b$. 
The system $Ax = b$ lacks a solution for some $b \in \mathbb{R}^m$ if and only if there exist such $b$ that do not belong to the column space of the matrix $A$, i.e., $\text{Col}(A) \subsetneq \mathbb{R}^m$. This is possible only if $\text{rank}(A|b) > \text{rank}(A)$ for some $b$, where $(A|b)$ denotes the augmented matrix formed by adding $b$ to $A$ as an additional column.

If $\text{rank}(A) < m$, then it is possible for there to exist such $b \in \mathbb{R}^m$ for which the system $Ax = b$ lacks a solution, since the rank of the main matrix is less than the number of rows, and therefore, not all $b$ can be represented as linear combinations of the columns of $A$.

For the system $Ax = b$, which lacks a solution for some $b \in \mathbb{R}^m$, it is necessary that the condition $r < m$ is satisfied.

### 3.4.B. $Ax = b$ has infinitely many solutions for every $b$.  
For the system $Ax = b$, where $A \in \text{Mat}_{m \times n}(\mathbb{R})$ and $b \in \mathbb{R}^m$, in order for there to exist infinitely many solutions for every $b$, the following conditions are necessary:

**Consistency for every $b$**: The system must be consistent for any $b$, requiring that $r = \text{rank}(A) = \text{rank}(A|b)$. This implies that any $b$ must lie within the space spanned by the columns of $A$. Since we desire this to hold for all $b \in \mathbb{R}^m$, we deduce that $r = m$.

**Indeterminacy**: To have infinitely many solutions, the number of variables must exceed the number of linearly independent equations, i.e., $n > r$.

From these conditions, it follows that for the system $Ax = b$ to have infinitely many solutions for every $b \in \mathbb{R}^m$, the relationship $r = m < n$ must hold.

### 3.4.C. $Ax = b$ has a unique solution for some $b$, no solution for other $b$.  

The system has a unique solution for some $b$ if $r = n$. This condition ensures the uniqueness of the solution by matching the number of linearly independent equations with the number of unknowns.

The system has no solution for other $b$ if $r < m$. This condition indicates that the space spanned by the columns of $A$ does not encompass all possible $b \in \mathbb{R}^m$, thereby implying the existence of such $b$ for which the system is inconsistent.

From these conditions, it follows that for the system $Ax = b$ to have a unique solution for some $b$ and no solution for other $b$, the relation $r = n < m$ must be satisfied. This denotes that the matrix $A$ must be of full column rank ($r = n$), but the number of equations ($m$) exceeds the number of unknowns ($n$), making the system underdetermined for some $b$ and overdetermined for others.
### 3.4.D. $Ax = b$ has a unique solution for every $b$.
Following relations must be satisfied:
- The system has a unique solution for all $b$, which is possible only when $A$ is invertible and hence square. This implies that $m = n$.
- For $A$ to be invertible, it must have full rank, which equates to the condition $r = n$.

Therefore, for the system $Ax = b$ to have a unique solution for every vector $b$, it is necessary and sufficient that the conditions $m = n$ and $r = m = n$ are met. This indicates that the matrix $A$ must be square and possess full rank.

### 3.5. Use Gauss – Jordan elimination to find the inverse for the matrix $(a, b, c \in K)$
$A = \begin{bmatrix} 1 & a & b \\ 0 & 1 & c \\ 0 & 0 & 1 \end{bmatrix}$

$[A|I] = \begin{bmatrix} 1 & a & b & | & 1 & 0 & 0 \\ 0 & 1 & c & | & 0 & 1 & 0 \\ 0 & 0 & 1 & | & 0 & 0 & 1 \end{bmatrix}$
$[A|I] = \begin{bmatrix} 1 & a & b & | & 1 & 0 & 0 \\ 0 & 1 & 0 & | & 0 & 1 & -c \\ 0 & 0 & 1 & | & 0 & 0 & 1 \end{bmatrix}$
$[A|I] = \begin{bmatrix} 1 & a & 0 & | & 1 & 0 & -b \\ 0 & 1 & 0 & | & 0 & 1 & -c \\ 0 & 0 & 1 & | & 0 & 0 & 1 \end{bmatrix}$
$[A|I] = \begin{bmatrix} 1 & 0 & 0 & | & 1 & -a & -b+a\cdot c \\ 0 & 1 & 0 & | & 0 & 1 & -c \\ 0 & 0 & 1 & | & 0 & 0 & 1 \end{bmatrix}$

$A^{-1} = \begin{bmatrix} 1 & -a & -b+a\cdot c \\ 0 & 1 & -c \\ 0 & 0 & 1 \end{bmatrix}$

