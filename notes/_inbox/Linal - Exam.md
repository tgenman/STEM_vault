# Linear Algebra
## Final Exam (Fall 2023)

### F.1.
Show that the rank of the sum of two $m$ by $n$ matrices is less than or equal to the sum of their ranks. Give an example of two matrices $A, B$ with $\text{rank}(A + B) = \text{rank} A + \text{rank} B$.

### F.2.
Let $K$ be a field. Denote by $K[x_1, \ldots, x_n]$ the $K$-algebra of polynomials in $n$ (commutative, independent) variables. Compute the dimension of the space $K[x_1, \ldots, x_n]_d$ of all homogeneous polynomials of degree equal to a given natural number $d$ as well as that of the space $K[x_1, \ldots, x_n]_{\leq d}$ of all polynomials of total degree less than or equal to $d$.

### F.3. (Fredholm alternative)
Let $\varphi : V \rightarrow V$ be a linear operator defined on an $n$-dimensional vector space $V$. Prove that exactly one of the following is true:
1. $\varphi$ is surjective.
2. $\dim \text{Ker} \varphi > 0$.

### F.4.
Let $K$ be a field of characteristic zero. Is it possible to find two $n$ by $n$ matrices $A$ and $B$ with entries in $K$ such that
$$AB - BA = I$$
($I$ is the identity matrix)?

### F.5.
Let $A$ be an $m$ by $n$ real matrix. Suppose $m > n$. Prove that $A^TA$ is not positive definite.

### F.6.
Let $A$ be a real symmetric positive definite matrix with its largest eigenvalue $\lambda_{\text{max}} < 1$. Prove that
$$\log \det A = \text{tr} \log A,$$
where the logarithm of the matrix $A$ is given by the power series
$$\log A = \sum_{k=1}^{\infty} (-1)^{k-1} \frac{(A - I)^k}{k}.$$

### F.7.
Suppose $A_n$ is a square matrix that has zeros on its main diagonal and minus ones elsewhere. Find $\det A_n$.

[Hint: One can proceed using linearity in rows – to that end a reasonable first step would be adding all rows except the last one to the last row. However, the quickest way is arguably via eigenvalues. For that, express the matrix as a sum of the identity matrix and a matrix whose spectrum can be easily studied.]

### F.8. (Householder reflector)
Let $v$ be a unit vector in $\mathbb{R}^n: v^Tv = 1$. Consider the following matrix:
$$H = I - 2vv^T$$
(its geometric meaning as an operator is reflection about a hyperplane through the origin specified by the normal vector $v$, hence the name). Prove that $H$ is symmetric and orthogonal, determine its eigenvalues, eigenvectors, its trace and determinant.

### F.9.
Suppose $A$ is a square matrix over the complex numbers. Prove that $A$ is similar to $A^T$.
[Hint: the first step is to verify the statement for the case of a single Jordan block $J$ – this was done in the assignments. The next step deals with the block-diagonal matrix comprised of multiple Jordan blocks – the matrix realizing the similarity will be assembled from blocks in a manner similar to the first step. To complete the proof, recall the definition of the Jordan form as a statement about the similarity between $A$ and a matrix of Jordan blocks.^1]

### F.10. (C. Mau, IMC)
Suppose $A$ is an $n \times n$ real matrix with real eigenvalues. Prove that if there exists an integer $k \geq n$ such that
$$A + A^k = A^T$$
then $A$ is necessarily the zero matrix.
[Hint: the first order of business is to prove that $A$ is nilpotent – or, equivalently, that the eigenvalues of $A$ are all zero. To that end, one may either prove that all the eigenvalues occur as roots of the polynomial $p(x) = x^k(1 + (1+x^{-1})^k)$ which can be seen to be relevant by transposing the identity from the hypothesis and plugging in $A^T$ (again from that defining identity); or go by contradiction, assuming there exists a non-zero $\lambda$ and either considering the maximal $|\lambda|$ or comparing the traces of $A^T$ and $A + A^T$. Once this is done, one will need to observe that $A$ must be symmetric, and therefore diagonalizable.]

---

^1 Here by degree we mean the standard degree function, i.e. the one with $\deg x_i = 1$ for every $i$.

