Linear Algebra  
(Fall 2023)  
Problem Set 4

Topics covered: properties of determinants.

4.1. Find the formula for the determinant of the matrix $A = [a_{ij}]$ with $a_{ij} = 0$ for $i < n - j + 1$ (i.e. the matrix $A$ has zeros above the antidiagonal).

4.2. Compute the determinant of the $n \times n$ matrices $F_{n+1}, n \geq 2$, which are defined as being tridiagonal, with ones on the main diagonal, ones on the diagonal below the main one, and minus ones on the diagonal above the main one. The three matrices following the one-by-one matrix $F_2 = [1]$ in the sequence have the form:

$$
F_3 = \begin{bmatrix}
1 & -1 & 0 \\
1 & 1 & -1 \\
0 & 1 & 1 
\end{bmatrix}, \quad
F_4 = \begin{bmatrix}
1 & -1 & 0 & 0 \\
1 & 1 & -1 & 0 \\
0 & 1 & 1 & -1 \\
0 & 0 & 1 & 1
\end{bmatrix}, \quad
F_5 = \begin{bmatrix}
1 & -1 & 0 & 0 & 0 \\
1 & 1 & -1 & 0 & 0 \\
0 & 1 & 1 & -1 & 0 \\
0 & 0 & 1 & 1 & -1 \\
0 & 0 & 0 & 1 & 1
\end{bmatrix}.
$$

[Hint: the letter "F" stands for Fibonacci.]

4.3. How will the determinant of an $n$ by $n$ matrix $A$ change when:

A. Every entry $a_{ij}$ is replaced by $-a_{ij}$.  
B. The rows $a_{1j}, a_{2j}, \ldots, a_{nj}$ of $A$ are permuted to $a_{nj}, a_{n-1,j}, \ldots, a_{1j}$.  
C. The columns $a_{i1}, a_{i2}, \ldots, a_{in}$ are permuted to $a_{i2}, \ldots, a_{in}, a_{i1}$.

4.4. Let $n$ be an odd number and let $A$ be a skew-symmetric $n$ by $n$ matrix. Show that $\text{det} A = 0$.

4.5. Prove that $\text{det} A$ (A has entries in a field $K$) is irreducible as a polynomial in the $n^2$ variables $a_{11}, a_{12}, \ldots, a_{nn}$.
