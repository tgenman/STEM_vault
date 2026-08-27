Linear Algebra  
(Fall 2023)  
Problem Set 7

Topics covered: eigenvalues and eigenvectors, Jordan form, Euclidean spaces and positive definite matrices.

7.1. Suppose $A$ is a $3 \times 3$ real matrix with eigenvalues $\{0,1,2\}$. Describe what (if anything) can be said about:

A. The rank of $A$.
B. The determinant of $A^TA$.
C. The eigenvalues of $A^TA$.
D. The eigenvalues of $(I + A^2)^{-1}$.

7.2. A. Prove that if a matrix $A$ is similar[1] to a diagonal matrix $\Lambda$, then $A^T$ is also similar to a diagonal matrix.

B. Given $S$ and $A$ corresponding to $A$ (in the situation of $A_\lambda$), what are the eigenvalues and eigenvectors of $A^T$?

7.3. Consider the matrix $A = A(\epsilon)$ depending on a parameter $\epsilon$:

$$
A = \begin{bmatrix}
1 & 1 \\
\epsilon & 1 
\end{bmatrix}.
$$

What can be said about the spectral properties (eigenvalues, eigenvectors and diagonalization, Jordan form) of $A$ for varying values of the parameter $\epsilon$? In particular, for which $\epsilon$ is $A$ similar to a diagonal matrix? What is the Jordan form of $A$ for the values of $\epsilon$ for which diagonalization is not possible?

7.4. Let $J(\lambda)$ be a Jordan block (i.e. a matrix with $\lambda$ on the main diagonal, ones on the diagonal above it and zeros elsewhere). Prove that $J^T$ is similar to $J[2]$.

7.5. Let $A$ be a real $n \times n$ symmetric positive definite matrix.

A. Prove that $A^{-1}$ exists and is symmetric positive definite.
B. Let $Q$ be an orthogonal $n \times n$ matrix. Prove that $Q^TAQ$ is symmetric positive definite.
C. Prove that the block matrix

$$
B = \begin{bmatrix}
A & A \\
A & A 
\end{bmatrix}
$$

is positive semidefinite but not positive definite.

---

[1]: That is, there is a matrix $S$ such that $A = S\Lambda S^{-1}$ thus $A$ and $\Lambda$ may be thought of as matrices of a certain linear operator in different bases.

[2]: Actually, this is the starting point of an argument that shows that every matrix $A$ that admits the Jordan form – in particular, every matrix $A$ over the complex numbers – is similar to its transpose $A^T$. The two other steps of the proof will be discussed in the final exam.
