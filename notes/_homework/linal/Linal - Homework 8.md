Linear Algebra  
(Fall 2023)  
Problem Set 8

Topics covered: singular value decomposition, pseudoinverse.

8.1. Let $A$ be the matrix

$$
A = \begin{bmatrix}
1 & 1 \\
1 & 0 
\end{bmatrix}.
$$

A. Find the eigenvalues and unit norm eigenvectors of $A^TA$ and $AA^T$.  
B. Use the previous result to construct the singular value decomposition for $A$.

8.2. For a matrix $A \in \mathbb{R}^{m \times n}$, the pseudoinverse $A^+$ of $A$ is defined as the matrix $A^+ \in \mathbb{R}^{n \times m}$ satisfying the following Moore – Penrose axioms:

1. $A^+A = A$.
2. $A^+AA^+ = A^+$.
3. $(A^+A)^T = A^+A$.
4. $(A^TA)^+ = A^+A$.

A. Prove that $(A^+)^+ = A$ and $A^+ = A^{-1}$ when $A$ is invertible.  
B. Verify that $A^T A$ and $AA^T$ are projection matrices. Describe the images of the two projections.  
C. Suppose $A$ has independent columns. Then $A^+ = (A^TA)^{-1}A^T$.  
D. Prove, using the defining axioms, that if the pseudoinverse $A^+$ exists then it is unique.

8.3. Let $A = U\Sigma V^T$ be the singular value decomposition of $A$.

A. Find $\Sigma^+$ (the pseudoinverse to $\Sigma$, see 8.2).  
B. Express $A^+$ via $U, V$ and $\Sigma^+$.  
C. Use the previous result together with 8.2D to conclude that for any matrix $A \in \mathbb{R}^{m \times n}$ the pseudoinverse $A^+$ exists and is unique.

8.4. A matrix norm on the set of (real, square) matrices $\mathbb{R}^{n \times n}$ is a function

$$\|\cdot\| : \mathbb{R}^{n \times n} \rightarrow \mathbb{R}$$

with the following properties:

1. $\|A\| \geq 0$ and $\|A\| = 0$ if and only if $A = 0$.
2. $\|aA\| = |a|\|A\|$ (for all $a \in \mathbb{R}$).
3. $\|A + B\| \leq \|A\| + \|B\|$.
4. $\|AB\| \leq \|A\|\|B\|$.

Prove that the following functions are matrix norms:

A. $\|\cdot\|_2 = \sigma_{\text{max}}(A)$ (the largest singular value of $A$, the spectral norm),  
B. $\|\cdot\|_F = \left(\sum_{i=1}^n \sum_{j=1}^n a_{ij}^2\right)^{\frac{1}{2}}$ (the Frobenius norm).

8.5. Let $A = CR$ denote the CR-decomposition of $A$. Suppose that the matrix $C \in \mathbb{R}^{m \times r}$ has full (column) rank $r$ and the matrix $R \in \mathbb{R}^{r \times n}$ has full (row) rank $r$. Prove that in this case the pseudoinverse $A^+$ of $A$ is

$$A^+ = R^+C^+.$$
