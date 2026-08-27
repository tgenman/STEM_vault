author: **Dmitrii Bondarev** (Дмитрий Бондарев)
group: М05-321сс (**Contemporary Combinatorics**)
date: 2024-02-06

### 2.1. Compute the reduced row echelon form
 of the matrix$A = \begin{bmatrix} 1 & 2 & 0 & 1 \\ -1 & 0 & 1 & 2 \\ 1 & -2 & 1 & 0\end{bmatrix}$. Write out the elementary matrices whose left action results in the reduced row echelon form of $A$.


$E_1 = \begin{bmatrix} 1 & 0 & 0 \\ 1 & 1 & 0 \\ 0 & 0 & 1\end{bmatrix}$     $E_1A = \begin{bmatrix} 1 & 2 & 0 & 1 \\ 0 & 2 & 1 & 3 \\ 1 & -2 & 1 & 0\end{bmatrix}$

$E_2 = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ -1 & 0 & 1\end{bmatrix}$   $E_2E_1A = \begin{bmatrix} 1 & 2 & 0 & 1 \\ 0 & 2 & 1 & 3 \\ 0 & -4 & 1 & -1\end{bmatrix}$

$E_3 = \begin{bmatrix} 1 & 0 & 0 \\ 0 & \frac{1}{2} & 0 \\ 0 & 0 & 1\end{bmatrix}$ $E_3E_2E_1A = \begin{bmatrix} 1 & 2 & 0 & 1 \\ 0 & 1 & \frac{1}{2} & \frac{3}{2} \\ 0 & -4 & 1 & -1\end{bmatrix}$

$E_4 = \begin{bmatrix} 1 & -2 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1\end{bmatrix}$ $E_4E_3E_2E_1A = \begin{bmatrix} 1 & 0 & -1 & -2 \\ 0 & 1 & \frac{1}{2} & \frac{3}{2} \\ 0 & -4 & 1 & -1\end{bmatrix}$

$E_5 = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 4 & 1\end{bmatrix}$ $E_5E_4E_3E_2E_1A = \begin{bmatrix} 1 & 0 & -1 & -2 \\ 0 & 1 & \frac{1}{2} & \frac{3}{2} \\ 0 & 0 & 3 & 5\end{bmatrix}$

$E_6 = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & \frac{1}{3}\end{bmatrix}$ $E_6E_5E_4E_3E_2E_1A = \begin{bmatrix} 1 & 0 & -1 & -2 \\ 0 & 1 & \frac{1}{2} & \frac{3}{2} \\ 0 & 0 & 1 & \frac{5}{3}\end{bmatrix}$


$E_7 = \begin{bmatrix} 1 & 0 & 1 \\ 0 & 1 & 0 \\ 0 & 0 & 1\end{bmatrix}$ $E_7E_6E_5E_4E_3E_2E_1A = \begin{bmatrix} 1 & 0 & 0 & -\frac{1}{3} \\ 0 & 1 & \frac{1}{2} & \frac{3}{2} \\ 0 & 0 & 1 & \frac{5}{3}\end{bmatrix}$

$E_8 = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & -\frac{1}{2} \\ 0 & 0 & 1\end{bmatrix}$ $E_8E_7E_6E_5E_4E_3E_2E_1A = \begin{bmatrix} 1 & 0 & 0 & -\frac{1}{3} \\ 0 & 1 & 0 & \frac{2}{3} \\ 0 & 0 & 1 & \frac{5}{3}\end{bmatrix}$


---

### 2.2. Find out which of the following subsets of $\text{Mat}_{n \times n}(K)$ form a group with respect to matrix multiplication:

#### 2.2.1 A. Lower triangular matrices with ones along the main diagonal
Satisfies the conditions
**Closure**
If $A$ and $B$ are two lower triangular matrices with ones on the main diagonal, then their product $AB$ is also a lower triangular matrix with ones on the main diagonal.
$A = \begin{bmatrix} 1 & 0 & 0 \\ a_{21} & 1 & 0 \\ a_{31} & a_{32} & 1 \\ \end{bmatrix}, \quad B = \begin{bmatrix} 1 & 0 & 0 \\ b_{21} & 1 & 0 \\ b_{31} & b_{32} & 1 \\\end{bmatrix}$

$AB = \begin{bmatrix} 1 & 0 & 0 \\ a_{21} + b_{21} & 1 & 0 \\ a_{31} + a_{32}b_{21} + b_{31} & b_{32} + a_{32} & 1 \\ \end{bmatrix}$


Let $A, B \in \mathbb{L}_n$ where $\mathbb{L}_n$ denotes the set of $n \times n$ lower triangular matrices with ones on the main diagonal. For $A = [a_{ij}]$ and $B = [b_{ij}]$, the $(i, j)$-th element of $AB$ is given by:

$(AB)_{ij} = \sum_{k=1}^{n} a_{ik}b_{kj}$

For $i < j$, $a_{ik} = 0$ for $k \geq i$ and $b_{kj} = 0$ for $k < j$, ensuring $(AB)_{ij} = 0$ for $i < j$, preserving lower triangularity. For $i = j$, $(AB)_{ij} = \sum_{k=1}^{n} a_{ik}b_{kj} = 1$ since $a_{ik} = b_{kj} = 1$ for $k = i = j$, preserving ones on the diagonal.

**Identity**
The identity element $E$ in $\mathbb{L}_n$ is the $n \times n$ identity matrix, which is a lower triangular matrix with ones on the main diagonal.

**Inverses**
Each lower triangular matrix $A$ with ones on the main diagonal has an inverse $A^{-1}$, which is also a lower triangular matrix with ones on the main diagonal. The inverse exists because the determinant of $A$ (the product of its diagonal elements) is non-zero (specifically, it is $1$), and the inverse can be constructed to preserve lower triangularity and ones on the diagonal.

**Associativity.** Matrix multiplication is inherently associative, a property that holds regardless of the matrices' specific types.

#### 2.2.2 B. Lower triangular matrices 
Fail inverse requirement:
- A matrix $A \in L$ is invertible iff all diagonal elements are non-zero, i.e., $\forall i, a_{ii} \neq 0$.
- $L$ includes matrices with $a_{ii} = 0$ for some $i$, making them non-invertible.
- For a set to be a group, every element must have an inverse in the set. However, $\exists A \in L$ such that $A^{-1} \notin L$ due to non-invertibility.
- Consequently, $L$ does not satisfy the group requirement for invertibility, $\nexists A^{-1}$ for all $A \in L$.
#### 2.2.3 C. Symmetric matrices.  
Fail closure requirement:
The product of two symmetric matrices is not always a symmetric matrix. As an example, consider two symmetric $3 \times 3$ matrices:
$A = \left[ \begin{matrix} 1 & 2 & 3 \\ 2 & 1 & 4 \\ 3 & 4 & 1 \end{matrix} \right], \quad B = \left[ \begin{matrix} 2 & 5 & 6 \\ 5 & 2 & 7 \\ 6 & 7 & 2 \end{matrix} \right]$

Both matrices $A$ and $B$ are symmetric, since $A = A^T$ and $B = B^T$. However, if we compute their product:
$AB = \left[ \begin{matrix} 1 & 2 & 3 \\ 2 & 1 & 4 \\ 3 & 4 & 1 \end{matrix} \right] \left[ \begin{matrix} 2 & 5 & 6 \\ 5 & 2 & 7 \\ 6 & 7 & 2 \end{matrix} \right] = \left[ \begin{matrix} 32 & 28 & 23 \\ 39 & 35 & 22 \\ 37 & 37 & 29 \end{matrix} \right]$

The resulting matrix $AB$ is not symmetric, demonstrating that the set of symmetric matrices is not closed under matrix multiplication.
#### 2.2.4 D. Diagonal invertible matrices. 
Satisfies the conditions

**Closure.** The product of any two invertible diagonal matrices $A$ and $B$ is also a diagonal matrix, where the diagonal entry in position $(i, i)$ is $a_{ii}b_{ii}$. Since $a_{ii}$ and $b_{ii}$ are nonzero (the matrices are invertible), their product $a_{ii}b_{ii}$ is also nonzero, ensuring $AB$ is an invertible diagonal matrix. Thus, the set is closed under multiplication.

**Identity Element.** The identity matrix $I_n$, with ones on its diagonal and zeros elsewhere, is a diagonal matrix and invertible (its own inverse). Thus, the identity element exists in the set.

**Inverse Element.** Let $A$ be an invertible diagonal matrix with diagonal entries $a_{11}, a_{22}, \ldots, a_{nn}$. Since $A$ is invertible, all $a_{ii} \neq 0$. The inverse $A^{-1}$ is also diagonal, with diagonal entries $1/a_{11}, 1/a_{22}, \ldots, 1/a_{nn}$. Hence, every element in the set has an inverse in the set.

**Associativity.** Matrix multiplication is inherently associative, a property that holds regardless of the matrices' specific types.
#### 2.2.5 E. Permutation matrices.  
Satisfies the conditions

**Closure.** For any two permutation matrices $A$ and $B$, there exists a permutation matrix $C$ such that $AB = C$. This follows because the operation of matrix multiplication for permutation matrices corresponds to the composition of permutations, and since the set of all permutations on a finite set is closed under composition, $\forall A, B \in G, \exists C \in G : AB = C$, where $G$ is the set of permutation matrices.

**Identity Element.** There exists an identity matrix $I_n$ such that for any permutation matrix $P$, $PI_n = I_nP = P$. This satisfies the requirement for an identity element in the group, $\exists I_n \in G, \forall P \in G: PI_n = I_nP = P$.

**Inverse Element.** For each permutation matrix $P$, there exists an inverse permutation matrix $P^{-1}$ such that $PP^{-1} = P^{-1}P = I_n$. This is because each permutation is bijective and has an inverse permutation, $\forall P \in G, \exists P^{-1} \in G: PP^{-1} = P^{-1}P = I_n$.

**Associativity.** Matrix multiplication is inherently associative, a property that holds regardless of the matrices' specific types.


#### 2.2.6 F. Matrices $A$ with $A^{-1} = A^T$.
Satisfies the conditions

**Closure.** For any two matrices $A$ and $B$ in the set, there exists a matrix $C$ in the set such that $AB = C$. Specifically, if $A^{-1} = A^T$ and $B^{-1} = B^T$, then for their product $AB$, we have $(AB)^{-1} = B^{-1}A^{-1} = B^TA^T = (AB)^T$. Therefore, $\forall A, B \in G, \exists C \in G : AB = C$ where $G$ is the set of matrices satisfying $A^{-1} = A^T$.

**Identity Element.** There exists an identity matrix $I$ in the set that satisfies $I^{-1} = I^T = I$. This ensures that for any matrix $A$ in the set, multiplying by the identity matrix does not alter $A$, i.e., $\exists I \in G, \forall A \in G: AI = IA = A$.

**Inverse Elements.** For each matrix $A$ in the set, there exists an inverse matrix $A^{-1}$, which equals $A^T$. Since matrix transposition is a bijective operation, the transposed matrix $A^T$ has an inverse which will also be $A$, ensuring $\forall A \in G, \exists A^{-1} \in G: AA^{-1} = A^{-1}A = I$.

**Associativity.** Matrix multiplication is inherently associative, a property that holds regardless of the matrices' specific types.

### 2.3. Prove that the general linear group $GL(n, K)$ is generated by elementary matrices.

To prove that $GL(n, K)$ is generated by elementary matrices, we need to show that any invertible matrix $A \in GL(n, K)$ can be expressed as a product of elementary matrices.

**Reduction to echelon form using elementary operations**: Any matrix $A$ can be reduced to echelon form using elementary row (or column) operations, which correspond to left multiplication by elementary matrices. Let $E_1, E_2, \ldots, E_k$ be elementary matrices such that $E_k \cdots E_2 E_1 A = U$, where $U$ is an echelon form matrix.

**Further reduction to the identity matrix**: The echelon form $U$ can be further reduced to the identity matrix $I$ using additional elementary operations, corresponding to multiplication by elementary matrices. Let $E_{k+1}, \ldots, E_m$ be such elementary matrices that $E_m \cdots E_{k+1} U = I$.

**Reversing the process**: Since each elementary operation is reversible, we can apply the inverse operations to the identity matrix to obtain $A$. That is, if $E_i^{-1}$ denotes the inverse of $E_i$, then $A = E_1^{-1} E_2^{-1} \cdots E_k^{-1} E_{k+1}^{-1} \cdots E_m^{-1} I$
Thus, $A$ can be represented as a product of elementary matrices and their inverses.

### 2.4. Prove that the factors $L, D$ and $U$ are uniquely defined
Let $A$ be a square matrix. If $A = L_0U_0$ is an LU factorization of $A$, then it can be transformed into $A = LDU$ with $D$ diagonal and $L, U$ having the non-zero entries along their main diagonals equal to 1 by taking $L_0 = LD_1, U_0 = D_2U$ ($D_1$ and $D_2$ are diagonal), $D = D_1D_2$. This form of LU factorization is called the lower-diagonal-upper (LDU) decomposition.

Let $A$ be invertible with $A = LDU$ its LDU decomposition[1] with all three factors invertible. Prove that the factors $L, D$ and $U$ are uniquely defined.

**Prove**

Suppose there are two different LDU decompositions for an invertible matrix $A$:
$A = LDU = L'D'U',$
where $L, D, U$ and $L', D', U'$ are different sets of matrices as described above.

Adjust it by multiplying both sides by the inverse of $U$ on the right and the inverse of $L$ on the left, we get:
$D = L^{-1}L'D'U'U^{-1}.$

Since the product $L^{-1}L'$ results in a lower triangular matrix with 1s on its diagonal, and $U'U^{-1}$ results in an upper triangular matrix with 1s on its diagonal, for $D$ to remain a diagonal matrix, $L^{-1}L'$ and $U'U^{-1}$ must both effectively be the identity matrix, $I$. This means $L = L'$ and $U = U'$.

Given that $L$ and $U$ are found to be unique, and since $A = LDU = L'D'U'$, it logically follows that $D$ must also be unique because $D = L^{-1}AU^{-1}$.

Therefore, for any invertible matrix $A$ with an LDU decomposition, the matrices $L$, $D$, and $U$ must be unique.

### 2.5. Prove that the reduced row echelon form of a matrix $A$ (over a field) is uniquely defined.

**Proof:**

To show that the RREF of a matrix $A$ (over a field) is uniquely determined, let's assume, for contradiction, that there are two distinct RREF matrices, $R$ and $R'$, both derived from the same matrix $A \in F^{m \times n}$ via Elementary Row Operations.

Since $R \neq R'$, there exists at least one element, say $(i, j)$, where $R_{ij} \neq R'_{ij}$.

Assuming without loss of generality that $R_{ij} = 1$ is a leading entry in row $i$ of $R$, and $R'_{ij} = 0$. Given $R_{ij} = 1$ as a leading entry, all elements in column $j$ of $R$, above and below it, must be $0$. For $R'_{ij}$ being $0$, and considering $R'$ is in RREF, this suggests two scenarios for column $j$ in $R'$:

1. There's a leading $1$ in some row $k$ with $k > i$. This conflicts with the RREF rule stating each leading $1$ must be above any all-zero rows, and no non-zero entry can be above a leading one.

2. Column $j$ lacks a leading $1$, contradicting the premise that $R$ and $R'$ share the same pivot positions derived from $A$. These pivot positions are fixed by the inherent row dependencies in $A$ and are unaltered by Elementary Row Operations.

This contradiction stems from the initial assumption that two distinct RREF matrices, $R$ and $R'$, could originate from $A$. The application of Elementary Row Operations doesn't change the row dependencies in $A$, meaning the pivot positions that dictate the leading $1$s in the RREF are determined by these dependencies and remain constant across any sequence of Elementary Row Operations, thereby proving the uniqueness of the RREF.



