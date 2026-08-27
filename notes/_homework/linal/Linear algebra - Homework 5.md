author: **Dmitrii Bondarev** (Дмитрий Бондарев)
group: М05-321сс (**Contemporary Combinatorics**)
date: 2024-02-11

### 5.1. 
Let $V$ be a vector space and let $U_1, \ldots, U_k$ be its subspaces. The system of subspaces $\{U_1, \ldots, U_k\}$ is linearly independent if the equality $u_1 + \ldots + u_k = 0$ (where $u_i \in U_i$) implies $u_1 = \ldots = u_k = 0$.

### 5.1.A. Prove that a system of two subspaces $\{U, W\}$ is linearly independent if and only if $U \cap W = \{0\}$
If $\{U, W\}$ is linearly independent, then $U \cap W = \{0\}$
Assume $\{U, W\}$ is linearly independent. Consider any vector $v \in U \cap W$. This implies $v$ belongs to both $U$ and $W$. By linear independence, the only way to obtain the zero vector from vectors in $U$ and $W$ (i.e., $u + w = 0$ for $u \in U$, $w \in W$) is if $u = w = 0$. Specifically, if $v$ and $-v$ are such that their sum is zero, then $v$ must be the zero vector. Hence, $U \cap W$ contains only the zero vector.

If $U \cap W = \{0\}$, then $\{U, W\}$ is linearly independent
Assume $U \cap W$ contains only the zero vector. Consider vectors $u \in U$ and $w \in W$ such that $u + w = 0$. We need to show $u = 0$ and $w = 0$. Since $u = -w$, and $w \in W$, $u$ also belongs to $W$ (as well as $U$), which contradicts our assumption unless $u = 0$. Consequently, $w = 0$ as $u + w = 0$. 

Thus, if $U \cap W = \{0\}$, any sum of vectors $u \in U$ and $w \in W$ equaling zero implies $u = w = 0$, proving $\{U, W\}$ is linearly independent.
### 5.1.B. Give an example of a system of three vector spaces such that it is linearly dependent and the intersection of every two elements of the system is the zero space.
Let $V = \mathbb{R}^3$. Define vectors $v_1 = (1, 0, 0)$, $v_2 = (0, 1, 0)$, and $v_3 = (-1, -1, 0)$ in $V$. Observe that $v_1 + v_2 + v_3 = 0$, indicating linear dependence among $v_1$, $v_2$, and $v_3$.

Define the subspaces $U_1, U_2, U_3 \subseteq V$ as follows:
- $U_1 = \langle v_1 \rangle = \{ \lambda v_1 \mid \lambda \in \mathbb{R} \}$,
- $U_2 = \langle v_2 \rangle = \{ \mu v_2 \mid \mu \in \mathbb{R} \}$,
- $U_3 = \langle v_3 \rangle = \{ \nu v_3 \mid \nu \in \mathbb{R} \}$.

It follows that:
1. $U_1 \cap U_2 = \{0\}$, $U_1 \cap U_3 = \{0\}$, and $U_2 \cap U_3 = \{0\}$, ensuring that the intersection of any two distinct subspaces is the zero space.
2. $\exists u_1 \in U_1, u_2 \in U_2, u_3 \in U_3$ such that $u_1 + u_2 + u_3 = 0$ and not all $u_i$ are zero, demonstrating the linear dependence of the system $\{U_1, U_2, U_3\}$. 

### 5.2. Let $K$ be an infinite field and let $V$ be a vector space over $K$. Prove that $V$ cannot be expressed as a union of finitely many proper subspaces. Show that the statement is not true over finite fields.
#### Part 1
Let $V$ be a vector space over an infinite field $K$. Assume, for the sake of contradiction, that $V$ can be expressed as the union of a finite number of its proper subspaces:
$V = U_1 \cup U_2 \cup \dots \cup U_n, \quad n \in \mathbb{N}$
where each $U_i$ is a proper subspace of $V$.

Select $v_1 \in U_1$ and $v_2 \in U_2$ such that $v_1 \neq 0$, $v_2 \neq 0$, and $v_1 \not\in U_2$, $v_2 \not\in U_1$ (if $U_1 = U_2$, one can choose $v_2$ from another $U_j$, $j \neq 1$).

Consider $v = v_1 + \lambda v_2$, where $\lambda \in K$. Since $K$ is infinite, there exist infinitely many distinct values of $\lambda$, and consequently, infinitely many distinct vectors $v$. This contradicts the assumption that $V$ is the union of a finite number of subspaces, as not all vectors $v$ can be covered by these subspaces.

Hence, it follows that $V$ cannot be expressed as the union of a finite number of its proper subspaces.

#### Part 2
Let's consider the vector space $V = \mathbb{F}_2^2$ over the finite field $\mathbb{F}_2$, which contains just two elements: $0$ and $1$. The field $\mathbb{F}_2$ is finite, and the elements of the vector space $V$ can be represented by all ordered pairs of elements from $\mathbb{F}_2$, i.e.,

$V = \{(0,0), (0,1), (1,0), (1,1)\}$

Define the subspaces of $V$ as follows:
1. $U_1 = \{(0,0), (0,1)\}$, lines parallel to the $x$-axis.
2. $U_2 = \{(0,0), (1,0)\}$, lines parallel to the $y$-axis.
3. $U_3 = \{(0,0), (1,1)\}$, the diagonal through the origin.

Then, $V$ can be expressed as the union of these subspaces:
$V = U_1 \cup U_2 \cup U_3$

Each element from $V$ is contained in at least one of the subspaces, demonstrating that $V$ can indeed be represented as the union of a finite number of its proper subspaces.

### 5.3. 
Let $V$ be the vector space $\text{Mat}_{n \times n}(\mathbb{R})$ of all square $n$ by $n$ matrices with real entries.

### 5.3.A. 
Prove that $V = S \oplus A$, where $S$ is the subspace of all symmetric matrices (i.e. matrices $A$ such that $A = A^T$, where $A^T$ is $A$ transposed), and $A$ is the subspace of all skew-symmetric matrices ($A = -A^T$).

Step 1: Unique Representation of Each Matrix $M \in V$
For any matrix $M$ in $V$, it can be uniquely represented as the sum of a symmetric matrix and a skew-symmetric matrix:
$M = \frac{1}{2}(M + M^T) + \frac{1}{2}(M - M^T)$

- The first part, $\frac{1}{2}(M + M^T)$, is symmetric since:
$\left(\frac{1}{2}(M + M^T)\right)^T = \frac{1}{2}(M^T + (M^T)^T) = \frac{1}{2}(M + M^T)$

- The second part, $\frac{1}{2}(M - M^T)$, is skew-symmetric since:
$\left(\frac{1}{2}(M - M^T)\right)^T = \frac{1}{2}(M^T - (M^T)^T) = \frac{1}{2}(M^T - M) = -\frac{1}{2}(M - M^T)$

Hence, every matrix $M \in V$ can be uniquely expressed as the sum of a symmetric and a skew-symmetric matrix.

2: Intersection of $S$ and $A$ Contains Only the Zero Matrix
Assume there exists a matrix $X$ that is both symmetric and skew-symmetric, i.e., $X = X^T$ and $X = -X^T$. The only matrix that satisfies both conditions is the zero matrix. To show this:
$X = X^T \quad \text{and} \quad X = -X^T \implies X = -X \implies 2X = 0 \implies X = 0.$

Therefore, the intersection $S \cap A$ consists only of the zero matrix, implying $S \cap A = \{0\}$.

### 5.3.B. 
Prove that $V = S \oplus U_0$, where $S$ is the subspace of symmetric matrices (as before), and $U_0$ is the subspace of all nil upper triangular matrices (i.e. matrices $A = [a_{ij}]$ such that $a_{ij} = 0$ for $i \geq j$).

1: Unique Decomposition of Each Matrix in $V$
Consider any matrix $M \in V$. We aim to find matrices $S \in S$ and $U \in U_0$ such that $M = S + U$.

Define the symmetric matrix $S$ with components:
- $s_{ij} = m_{ij}$ for $i \leq j$,
- $s_{ij} = m_{ji}$ for $i > j$.

This ensures $S$ is symmetric since $s_{ij} = s_{ji}$ for all $i, j$.

Define $U = M - S$. Given $S$'s symmetry, $U$ will have zeros on and below its diagonal, making it a member of $U_0$ by having nilpotent properties above the diagonal. This proves any $M \in V$ can be uniquely decomposed into $S + U$, where $S \in S$ and $U \in U_0$.

2: Intersection of $S$ and $U_0$ Is Only the Zero Matrix
Suppose there exists a matrix $X \in S \cap U_0$. Since $X \in S$, $X$ is symmetric. As $X \in U_0$, $X$ is an upper triangular matrix with zeros on and below its diagonal. The only matrix that is both symmetric and has this form of upper triangularity is the zero matrix. Hence, $S \cap U_0 = \{0\}$.

### 5.3.C. 
Prove that $V = A \oplus U$ where $A$ is the subspace of skew-symmetric matrices (as before) and $U$ is the space of all upper triangular matrices.

### 5.4. 
Let $f : V \rightarrow K$ be a non-zero linear function on a vector space $V$ (which is not assumed to be finite-dimensional) and let $U = \text{Ker}(f)$ be its kernel. Prove the following statements:

### 5.4.A. There is no subspace $W \subseteq V$ such that $U \subsetneq W \subsetneq V$ (strict inclusions).
To prove the statement, let's proceed by contradiction. Assume there exists a subspace $W$ such that $U \subsetneq W \subsetneq V$, where $U = \text{Ker}(f)$.

Given $W$ is strictly larger than $U$, there exists $w \in W$ not in $U$, implying $f(w) \neq 0$. For any $v \in V$, our goal is to show $v$ can be expressed using elements from $W$, contradicting the assumption $W \subsetneq V$.

Consider the linear mapping $f(v) = k$ for some $k \in K$. Define $v' = v - \frac{k}{f(w)}w$. Observe that:
$f(v') = f(v) - \frac{k}{f(w)}f(w) = k - k = 0$
indicating $v' \in U$, and since $U \subseteq W$, it follows $v' \in W$.

Therefore, $v$ can be represented as $v = v' + \frac{k}{f(w)}w$, where both terms belong to $W$ ($v'$ is in $W$ because $v' \in U \subseteq W$, and $w$ is chosen from $W$). This implies every $v \in V$ can be represented through elements of $W$, contradicting the premise that $W$ is strictly smaller than $V$.

Hence, our initial assumption is false, and no such subspace $W$ exists, proving the statement.


