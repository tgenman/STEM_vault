author: **Dmitrii Bondarev** (Дмитрий Бондарев)
group: М05-321сс (**Contemporary Combinatorics**)
date: 2024-02-05

### 1.1.A Compute the following matrix products:

$A = \left[ \begin{matrix} \cos \alpha & -\sin \alpha \\ \sin \alpha & \cos \alpha \end{matrix} \right]^n$

This is rotation matrix
$A^n = \left[ \begin{matrix} \cos(n\alpha) & -\sin(n\alpha) \\ \sin(n\alpha) & \cos(n\alpha) \end{matrix} \right]$

Prove it.

**Base Case**
For $n=1$, clearly, $A^1 = A$, which matches our formula.

**Inductive Step**
Assume the formula holds for $n=k$; that is,
$A^k = \left[ \begin{matrix} \cos(k\alpha) & -\sin(k\alpha) \\ \sin(k\alpha) & \cos(k\alpha) \end{matrix} \right]$

We need to show it holds for $n=k+1$:
$A^{k+1} = A^k \cdot A = \left[ \begin{matrix} \cos(k\alpha) & -\sin(k\alpha) \\ \sin(k\alpha) & \cos(k\alpha) \end{matrix} \right] \cdot \left[ \begin{matrix} \cos \alpha & -\sin \alpha \\ \sin \alpha & \cos \alpha \end{matrix} \right]$

$A^{k+1} = \left[ \begin{matrix} \cos(k\alpha)\cos(\alpha) - \sin(k\alpha)\sin(\alpha) & -(\cos(k\alpha)\sin(\alpha) + \sin(k\alpha)\cos(\alpha)) \\ \sin(k\alpha)\cos(\alpha) + \cos(k\alpha)\sin(\alpha) & \cos(k\alpha)\cos(\alpha) - \sin(k\alpha)\sin(\alpha) \end{matrix} \right]$

By using trigonometric identities
$\cos(a+b) = \cos(a)\cos(b) - \sin(a)\sin(b)$ and $\sin(a+b) = \sin(a)\cos(b) + \cos(a)\sin(b)$, 
we simplify the above expression to
$A^{k+1} = \left[ \begin{matrix} \cos((k+1)\alpha) & -\sin((k+1)\alpha) \\ \sin((k+1)\alpha) & \cos((k+1)\alpha) \end{matrix} \right]$



---
$B = \left[ \begin{matrix} \lambda & 1 \\ 0 & \lambda \end{matrix} \right]^n$

- For $n=1$, $B^1 = B$.
- For $n=2$, we multiply $B$ by itself:
$B^2 = B \cdot B = \left[ \begin{matrix} \lambda & 1 \\ 0 & \lambda \end{matrix} \right] \cdot \left[ \begin{matrix} \lambda & 1 \\ 0 & \lambda \end{matrix} \right] = \left[ \begin{matrix} \lambda^2 & 2\lambda \\ 0 & \lambda^2 \end{matrix} \right]$

- For $n=3$, multiplying $B^2$ by $B$:

$B^3 = B^2 \cdot B = \left[ \begin{matrix} \lambda^2 & 2\lambda \\ 0 & \lambda^2 \end{matrix} \right] \cdot \left[ \begin{matrix} \lambda & 1 \\ 0 & \lambda \end{matrix} \right] = \left[ \begin{matrix} \lambda^3 & 3\lambda^2 \\ 0 & \lambda^3 \end{matrix} \right]$

$B^n = \left[ \begin{matrix} \lambda^n & n\lambda^{n-1} \\ 0 & \lambda^n \end{matrix} \right].$

---


$\left( \left[ \begin{matrix} 2 & 1 \\ 5 & 3 \\ \end{matrix} \right] \cdot \left[ \begin{matrix} 1 & 0 \\ 1 & 1 \\ \end{matrix} \right] \cdot \left[ \begin{matrix} 3 & -1 \\ -5 & 2 \\ \end{matrix} \right] \right)^n$


- Matrix $A = \left[ \begin{matrix} 2 & 1 \\ 5 & 3 \\ \end{matrix} \right]$
- Matrix $B = \left[ \begin{matrix} 1 & 0 \\ 1 & 1 \\ \end{matrix} \right]$ raises to the power of $n$: $B^n = \left[ \begin{matrix} 1 & 0 \\ n & 1 \end{matrix} \right]$
- Matrix $C = \left[ \begin{matrix} 3 & -1 \\ -5 & 2 \\ \end{matrix} \right]$

To solve $(ABC)^n = ABCABCABC\ldots$ with the observation that $CA=I$ (the identity matrix),  simplify the expression to $A \cdot B^n \cdot C$.

$A \cdot B^n = \left[ \begin{matrix} 2 & 1 \\ 5 & 3 \\ \end{matrix} \right] \cdot \left[ \begin{matrix} 1 & 0 \\ n & 1 \end{matrix} \right] = \left[ \begin{matrix} 2 + n & 1 \\ 5 + 3n & 3 \end{matrix} \right]$

$(A \cdot B^n) \cdot C = \left[ \begin{matrix} 2 + n & 1 \\ 5 + 3n & 3 \end{matrix} \right] \cdot \left[ \begin{matrix} 3 & -1 \\ -5 & 2 \end{matrix} \right] = \left[ \begin{matrix} 1 + 3n & -n \\ 9n & 1 - 3n \end{matrix} \right]$

$(ABC)^n = \left[ \begin{matrix} 14n + 3 & -5n - 1 \\ 42n - 5 & 2 - 15n \end{matrix} \right]$


### 1.1.B
Given a square matrix $A$ and a polynomial $f(t) = a_0 + a_1t + \ldots + a_kt^k$ in one variable (both over $K$), the notation $f(A)$ stands for the matrix $f(A) = a_0I + a_1A + \ldots + a_kA^k$ (I is the identity matrix of the same size as $A$). Suppose $A$ and $C$ are square matrices of the same size and $C$ is invertible. Prove that $f(CAC^{-1}) = Cf(A)C^{-1}$.


**Applying $f(t)$ to $CAC^{-1}$**:
$f(CAC^{-1}) = a_0I + a_1(CAC^{-1}) + \ldots + a_k(CAC^{-1})^k$

$(CAC^{-1})^k = CAC^{-1}CAC^{-1}\ldots CAC^{-1} = CA^kC^{-1}$ because $C^{-1}C = I$.

$f(CAC^{-1}) = a_0I + a_1CAC^{-1} + \ldots + a_kCA^kC^{-1}$

$f(CAC^{-1}) = C(a_0I + a_1A + \ldots + a_kA^k)C^{-1} = Cf(A)C^{-1}$

This demonstrates that $f(CAC^{-1}) = Cf(A)C^{-1}$, which concludes the proof. 

---

### 1.2. 
#### 1.2.1  A. Let $A$ be a matrix. Find the matrix $E_{ij}A$
Formal definition of matrix multiplication

$c_{ik} = \sum_{r=1}^{m} e_{ir}a_{rk}$

Example
$E_{21}A = \left[ \begin{matrix} 0 & 0 & 0 \\ 1 & 0 & 0 \\ 0 & 0 & 0 \end{matrix} \right] \left[ \begin{matrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{matrix} \right] = \left[ \begin{matrix} 0 & 0 & 0 \\ a_{11} & a_{12} & a_{13} \\ 0 & 0 & 0 \end{matrix} \right]$

Multiplying $E_{ij}$ by $A$  copies the  $j$-th row of $A$ into the$i$-th row of the resulting matrix $C$, while setting all other elements to zero.


#### 1.2.2  B. Let $A$ be a matrix. Find the matrix $AE_{ij}$.
As in previous task
$AE_{21} = \left[ \begin{matrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{matrix} \right] \left[ \begin{matrix} 0 & 0 & 0 \\ 1 & 0 & 0 \\ 0 & 0 & 0 \end{matrix} \right] = \left[ \begin{matrix} a_{12} & 0 & 0 \\ a_{22} & 0 & 0 \\ a_{32} & 0 & 0 \end{matrix} \right]$

Multiplying $A$ by $E_{ij}$  copies the $i$-th column of $A$ into the $j$-th column of the resulting matrix $C$, while setting all other elements to zero.

#### 1.2.3   C. Let $A$ be a square matrix such that for all $i, j$ one has $E_{ij}A = AE_{ij}$. Prove that $A$ is a scalar matrix, i.e. $A = \lambda I$ (I is the identity matrix) for some $\lambda \in K$.
$E_{21}A = \left[ \begin{matrix} 0 & 0 & 0 \\ a_{11} & a_{12} & a_{13} \\ 0 & 0 & 0 \end{matrix} \right]$ $AE_{21} = \left[\begin{matrix} a_{12} & 0 & 0\\a_{22} & 0 & 0\\a_{32} & 0 & 0\end{matrix}\right]$

**Demonstrate that all off-diagonal elements of $A$ are $0$.**
Assume $i \neq j$. The multiplication $E_{ij}A$ results in a matrix where all elements are $0$ except for the $i$-th row, which is equivalent to the $j$-th row of matrix $A$. Similarly, the multiplication $AE_{ij}$ produces a matrix where all elements are $0$ except for the $j$-th column, which is equivalent to the $i$-th column of matrix $A$. Given that $E_{ij}A = AE_{ij}$, this is only possible if $a_{mn}=0$ for all $m \neq n$, i.e., all off-diagonal elements of matrix $A$ are $0$.

**Show that all diagonal elements of $A$ are equal to each other.**
Consider the case when $i = j$. The matrix $E_{ii}$ has a $1$ at position $(i, i)$ and zeros elsewhere. Multiplication $E_{ii}A$ yields a matrix where all elements except for the $i$-th row are zero, and similarly for $AE_{ii}$. As this equality holds for all $i$, it is only possible if all diagonal elements of matrix $A$ are equal to each other, i.e., $a_{11} = a_{22} = \dots = a_{nn} = \lambda$, for some $\lambda \in K$.

Therefore, $A$ is a scalar matrix of the form $A = \lambda I$, where $I$ is the identity matrix, and $\lambda$ is the common value of all diagonal elements of $A$.

#### 1.2.4 D. Recall that for a group $G$, its center $Z(G)$ is the set of all $h \in G$ such that $h$ commutes with every element $g \in G$: $gh = hg$. What is the center of $GL_n(K)$?
The center of the group $GL_n(K)$, denoted as $Z(GL_n(K))$, includes matrices $Z$ that commute with every matrix $A$ in $GL_n(K)$, meaning $ZA = AZ$ holds for any $A$.

Suppose $Z$ is a diagonal matrix with diagonal entries $z_{ii}$. Since a diagonal matrix commutes with any other diagonal matrix, and every matrix in $GL_n(K)$ can be represented as a product of elementary and diagonal matrices, $Z$ must at least commute with the diagonal matrices in $GL_n(K)$.

Considering a permutation matrix $P$ that swaps two rows, for $Z$ to commute with $P$, it must be symmetric to this swap, which is only possible if all diagonal elements of $Z$ are equal.

From these considerations, it follows that $Z$ must be a scalar matrix of the form $λI$, where $λ \in K \setminus \{0\}$, and $I$ is the identity matrix. Thus, $Z(GL_n(K)) = \{λI \,|\, λ \in K \setminus \{0\}\}$
#### 1.2.5 E. Let $A$ be a square matrix such that for all $i$ one has $E_{ii}A = AE_{ii}$. Prove that $A$ is a diagonal matrix.

$E_{11} = \left[\begin{matrix}1 & 0 & 0\\0 & 0 & 0\\0 & 0 & 0\end{matrix}\right]$ $A = \left[\begin{matrix}a_{11} & a_{12} & a_{13}\\a_{21} & a_{22} & a_{23}\\a_{31} & a_{32} & a_{33}\end{matrix}\right]$

$E_{11}A = \left[\begin{matrix}a_{11} & a_{12} & a_{13}\\0 & 0 & 0\\0 & 0 & 0\end{matrix}\right], \quad AE_{11} = \left[\begin{matrix}a_{11} & 0 & 0\\a_{21} & 0 & 0\\a_{31} & 0 & 0\end{matrix}\right]$
To ensure the equality $E_{11}A = AE_{11}$ holds, it is required that $a_{12} = a_{13} = a_{21} = a_{31} = 0$. Similarly, by considering $E_{22}A = AE_{22}$ and $E_{33}A = AE_{33}$, we conclude that all off-diagonal elements must be zero.

**Proof**

Suppose $A$ is an $n \times n$ square matrix, and for all $i$, the condition $E_{ii}A = AE_{ii}$ is satisfied. This implies that multiplying by $E_{ii}$ from either side isolates the $i$-th row or the $i$-th column of matrix $A$, respectively.

1. Multiplying by $E_{ii}$ from the left, $E_{ii}A$, zeros out all elements except those in the $i$-th row, leaving the $i$-th row unchanged from $A$.
2. Conversely, multiplying by $E_{ii}$ from the right, $AE_{ii}$, zeros out all elements except those in the $i$-th column, leaving the $i$-th column as in $A$.

For $E_{ii}A = AE_{ii}$ to hold, it is necessary for off-diagonal elements to be zero because otherwise, it would be impossible to achieve equality between the two multiplication results—one having non-zero elements solely in a row and the other solely in a column.

Therefore, all elements of matrix $A$, not on the main diagonal, must be zero. This implies that $A$ is a diagonal matrix.

---
### 1.3 Prove for all square matrices $A, B, C$ (of the same size) the following identities:
For two square matrices of the same size $A$ and $B$, denote by $[A, B]$ their commutator: 
$[A, B] = AB - BA.$

#### 1.3.1 $[A, BC] = [A, B]C + B[A, C]$
The left side of the equation is:
$[A, BC] = A(BC) - (BC)A = ABC - BCA$

The right side of the equation is:
$[A, B]C + B[A, C] = (AB - BA)C + B(AC - CA) = ABC - BAC + BAC - BCA =$
$= ABC - BCA = [A, BC]$

#### 1.3.2 $[[A, B], C] + [[B, C], A] + [[C, A], B] = 0$

Compute each commutator separately:
 $[[A, B], C] = [AB - BA, C] = (AB - BA)C - C(AB - BA) =$
 $= ABC - BAC - CAB + CBA$
 
$[[B, C], A] = [BC - CB, A] = (BC - CB)A - A(BC - CB) =$
$= BCA - CBA - ABC + ACB$

$[[C, A], B] = [CA - AC, B] = (CA - AC)B - B(CA - AC) =$
$= CAB - ACB - BCA + BAC$

Sum up it. All terms will cancel out:
$ABC - BAC - CAB + CBA + BCA - CBA -$
$- ABC + ACB + CAB - ACB - BCA + BAC = 0$

---

### 1.4. Prove that if a real matrix $A$ is normal and upper triangular then $A$ is diagonal.
Let $A \in \text{Mat}_{n \times n}(\mathbb{R})$ be a real square $n$ by $n$ matrix. $A$ is called normal if it commutes with its transpose: $[A^T, A] = 0.$

**Proof**:
Definition of a normal matrix: 
$A$ is normal if $AA^T = A^TA$. 

$A$ is an upper triangular matrix, and its transpose $A^T$, which would be a lower triangular matrix, 

For $A$ to be normal, the equality $AA^T = A^TA$ implies that every element outside the diagonal in $A$ must not contribute to any non-diagonal entries in the resulting matrix, for the resulting matrices to be identical. This condition can only be satisfied if the off-diagonal entries in $A$ are zero. 

Because: 
- The diagonal entries of $AA^T$ and $A^TA$ are sums of squares of the elements in the rows and columns of $A$, respectively. These sums will be equal for both products because they are just rearrangements of the same terms.
- For the off-diagonal elements, if $A$ has any non-zero off-diagonal term, the symmetry of the operation ($AA^T$ vs. $A^TA$) would not hold because the placement of non-zero off-diagonal elements would contribute differently to $AA^T$ and $A^TA$, violating the normality condition.

Thus, having non-zero off-diagonal elements in an upper triangular $A$ would prevent $A$ from being normal, as it would disrupt the equality $AA^T = A^TA$. Therefore, all off-diagonal elements must be zero for $A$ to satisfy the normality condition, leaving $A$ as a diagonal matrix.

---
### 1.5. 
Let $K$ be the field $\mathbb{R}$ of real numbers. Consider the $\mathbb{R}$-algebra $\text{Mat}_{2 \times 2}(\mathbb{R})$. Prove that the subset of $\text{Mat}_{2 \times 2}(\mathbb{R})$ consisting of all matrices of the form $\begin{bmatrix} a & -b \\b & a \end{bmatrix}$ is a subalgebra of $\text{Mat}_{2 \times 2}(\mathbb{R})$ isomorphic (as a real algebra) to the algebra $\mathbb{C}$ of complex numbers.

1. Show $S$ is Closed under Addition and Scalar Multiplication
**Addition:** Consider two matrices $A, B \in S$ where $A = \begin{bmatrix} a & -b \\ b & a \end{bmatrix}$ and $B = \begin{bmatrix} c & -d \\ d & c \end{bmatrix}$. Their sum is:
$A + B = \begin{bmatrix} a & -b \\ b & a \end{bmatrix} + \begin{bmatrix} c & -d \\ d & c \end{bmatrix} = \begin{bmatrix} a+c & -(b+d) \\ b+d & a+c \end{bmatrix}$

This is still of the form $\begin{bmatrix} x & -y \\ y & x \end{bmatrix}$, so $A + B \in S$.

**Scalar Multiplication:** Let $k \in \mathbb{R}$ and $A \in S$. Then $kA = k\begin{bmatrix} a & -b \\ b & a \end{bmatrix} = \begin{bmatrix} ka & -kb \\ kb & ka \end{bmatrix}$ so, $kA \in S$.

2. Show $S$ is Closed under Matrix Multiplication

Consider two matrices $A, B \in S$ as defined above. Their product is:

$AB = \begin{bmatrix} a & -b \\ b & a \end{bmatrix} \begin{bmatrix} c & -d \\ d & c \end{bmatrix} = \begin{bmatrix} ac-bd & -(ad+bc) \\ ad+bc & ac-bd \end{bmatrix}$

This product is of the form $\begin{bmatrix} x & -y \\ y & x \end{bmatrix}$, so $AB \in S$.

3. Show Existence of Multiplicative Identity in $S$

The multiplicative identity in $\text{Mat}_{2 \times 2}(\mathbb{R})$ is $I = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}$. Notice that this is of the form $\begin{bmatrix} a & -b \\ b & a \end{bmatrix}$ with $a=1$ and $b=0$, so $I \in S$.

4. Establish Isomorphism to $\mathbb{C}$

Define a mapping $\varphi: S \rightarrow \mathbb{C}$ by $\varphi\left(\begin{bmatrix} a & -b \\ b & a \end{bmatrix}\right) = a + bi$. We need to show that this mapping is an isomorphism.

- **Bijective**: It's clear that $\phi$ is injective (one-to-one) because different complex numbers map to different matrices. It's surjective (onto) because every matrix of the form $\begin{bmatrix} a & -b \\b & a \end{bmatrix}$ is the image of some complex number $a + bi$.
- **Preserves Addition**: $\phi((a + bi) + (c + di)) = \phi((a+c) + (b+d)i) = \begin{bmatrix} a+c & -(b+d) \\b+d & a+c \end{bmatrix}$, which matches the result of adding the matrices corresponding to $a + bi$ and $c + di$.
- **Preserves Multiplication**: $\phi((a + bi)(c + di)) = \phi((ac-bd) + (ad+bc)i) = \begin{bmatrix} ac-bd & -(ad+bc) \\ad+bc & ac-bd \end{bmatrix}$, which matches the result of multiplying the matrices corresponding to $a + bi$ and $c + di$.

