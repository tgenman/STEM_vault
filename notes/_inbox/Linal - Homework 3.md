
Linear Algebra  
(Fall 2023)  
Problem Set 3

Topics covered: vector spaces, bases, rank, the four fundamental subspaces.

3.1. (Yet another numerical example) Let $A$ be the matrix

$$
A = \begin{bmatrix}
0 & 1 & 2 & 1 \\
0 & -1 & 0 & 1 \\
0 & 1 & -1 & -2
\end{bmatrix}.
$$

A. Describe the nullspace $N(A)$ of the matrix $A$.  
B. Describe the column space $C(A)$ of $A$ (not just as the space of linear combinations of columns as per the definition, but rather as a subspace of $\mathbb{R}^3$ spanned by an appropriate linearly independent system).  
C. What is the reduced row echelon form $\text{rref}(A)$ of $A$?  
D. Consider the following block matrix $B$:

$$
B = \begin{bmatrix}
A & A \\
A & A
\end{bmatrix}.
$$

What is the reduced row echelon form $\text{rref}(B)$ of $B$?

3.2. Let $K = \mathbb{F}_q$ be a finite field with $q$ elements. Find the number of $k$-dimensional subspaces in a vector space $V$ of dimension $n$ over $K^{[1]}$.

3.3. Let $A$ and $B$ be matrices over a field $K$ of size $m \times n$ and $m \times k$, respectively. Show that the matrix equation

$$
AX = B
$$

where the unknown matrix $X$ has size $n \times k$ has a solution if and only if the rank of the matrix $A$ coincides with the rank of the augmented matrix

$$
[A|B].
$$

3.4. Let $A \in \text{Mat}_{m \times n}(\mathbb{R})$ and let $Ax = b$ be a linear system. Denote by $r$ the rank of $A$. Write down all known relations between $r, m, n$ in the following cases:

A. $Ax = b$ has no solution for some $b$.  
B. $Ax = b$ has infinitely many solutions for every $b$.  
C. $Ax = b$ has a unique solution for some $b$, no solution for other $b$.  
D. $Ax = b$ has a unique solution for every $b$.

3.5. Use Gauss – Jordan elimination to find the inverse for the matrix $(a, b, c \in K)$

$$
A = \begin{bmatrix}
1 & a & b \\
0 & 1 & c \\
0 & 0 & 1
\end{bmatrix}.
$$

[1]: This number is customarily denoted by $\binom{n}{k}$, and is referred to as the Gaussian binomial coefficient.
