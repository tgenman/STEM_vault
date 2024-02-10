
Linear Algebra  
(Fall 2023)  
Problem Set 5

Topics covered: vector spaces, linear maps.  
Note: The Axiom of Choice is assumed throughout the course.

5.1. Let $V$ be a vector space and let $U_1, \ldots, U_k$ be its subspaces. The system of subspaces $\{U_1, \ldots, U_k\}$ is linearly independent if the equality $u_1 + \ldots + u_k = 0$ (where $u_i \in U_i$) implies $u_1 = \ldots = u_k = 0$.

A. Prove that a system of two subspaces $\{U, W\}$ is linearly independent if and only if $U \cap W = \{0\}$.

B. Give an example of a system of three vector spaces such that it is linearly dependent and the intersection of every two elements of the system is the zero space.

5.2. Let $K$ be an infinite field and let $V$ be a vector space over $K$. Prove that $V$ cannot be expressed as a union of finitely many proper subspaces. Show that the statement is not true over finite fields.

5.3. Let $V$ be the vector space $\text{Mat}_{n \times n}(\mathbb{R})$ of all square $n$ by $n$ matrices with real entries.

A. Prove that $V = S \oplus A$, where $S$ is the subspace of all symmetric matrices (i.e. matrices $A$ such that $A = A^T$, where $A^T$ is $A$ transposed), and $A$ is the subspace of all skew-symmetric matrices ($A = -A^T$).

B. Prove that $V = S \oplus U_0$, where $S$ is the subspace of symmetric matrices (as before), and $U_0$ is the subspace of all nil upper triangular matrices (i.e. matrices $A = [a_{ij}]$ such that $a_{ij} = 0$ for $i \geq j$).

C. Prove that $V = A \oplus U$ where $A$ is the subspace of skew-symmetric matrices (as before) and $U$ is the space of all upper triangular matrices.

5.4. Let $f : V \rightarrow K$ be a non-zero linear function on a vector space $V$ (which is not assumed to be finite-dimensional) and let $U = \text{Ker}(f)$ be its kernel. Prove the following statements:

A. There is no subspace $W \subseteq V$ such that $U \subsetneq W \subsetneq V$ (strict inclusions). [1]

B. For every $x \notin U, V = U \oplus \text{span}(x)$.

5.5. Let $V$ be an infinite-dimensional vector space over a field $K$ and let $\text{dim} V$ denote the cardinality of a basis of $V$. Let $V^* = \text{Hom}(V, K)$ be its dual space. Prove that $\text{dim} V^* > \text{dim} V$.


[1]: This symbol denotes a proper subset.