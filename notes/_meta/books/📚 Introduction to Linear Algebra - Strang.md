---
aliases:
  - 📚 Введение в линейную алгебру
tags:
  - meta/book📚/classbook📖
  - meta/status/IN_PROGRESS_🌿
connected:
  - "[[Linear algebra (field)]]"
author:
  - "[[👤 Strang, Gilbert]]"
created: 2024-01-13 18:26
family: "[[🎓 18.06SC Linear Algebra - Strang]]"
---



**THE MATRIX ALPHABET**

- ${A}$ Any Matrix  
- ${B}$ Basis Matrix  
- ${C}$ Cofactor Matrix  
- ${D}$ Diagonal Matrix  
- ${E}$ Elimination Matrix  
- ${F}$ Fourier Matrix  
- ${H}$ Hadamard Matrix  
- ${I}$ Identity Matrix  
- ${J}$ Jordan Matrix  
- ${K}$ Stiffness Matrix  
- ${L}$ Lower Triangular Matrix  
- ${M}$ Markov Matrix  
- ${N}$ Nullspace Matrix  
- ${P}$ Permutation Matrix  
- ${P}$ Projection Matrix  
- ${Q}$ Orthogonal Matrix  
- ${R}$ Upper Triangular Matrix  
- ${R}$ Reduced Echelon Matrix  
- ${S}$ Symmetric Matrix  
- ${T}$ Linear Transformation  
- ${U}$ Upper Triangular Matrix  
- ${U}$ Left Singular Vectors  
- ${V}$ Right Singular Vectors  
- ${X}$ Eigenvector Matrix  
- ${\Lambda}$ Eigenvalue Matrix  
- ${\Sigma}$ Singular Value Matrix

### Линейное отображение

Отображение $T: V \to W$ между векторными пространствами над полем $F$ называется линейным, если для любых $u, v \in V$ и любого $\alpha \in F$ выполняются условия $T(u+v)=T(u)+T(v)$ и $T(\alpha u)=\alpha T(u)$.

### Линейный функционал

Линейным функционалом называется линейное отображение $f: V \to F$ из векторного пространства $V$ в поле скаляров $F$, то есть такое отображение, для которого для любых $u, v \in V$ и любого $\alpha \in F$ выполняются условия $f(u+v)=f(u)+f(v)$ и $f(\alpha u)=\alpha f(u)$.

### Функционал

Функционалом называется отображение $f: V \to F$ из векторного пространства $V$ в поле скаляров $F$, которое каждому вектору $v \in V$ сопоставляет одно число $f(v) \in F$.


### Лемма про сохранение линейного функционала
Если линейный функционал равен 0 на базисных векторах подпространства —  он равен 0 на всём подпространстве.

Если $f: V \to F$ — линейный функционал и $U \subset V$ — подпространство с базисом ${u_1,\dots,u_k}$, такое что $f(u_i)=0$ для всех $i$, то $f(u)=0$ для любого $u \in U$.

---

если обойти треугольник по сторонам, вернёшься в исходную точку, значит сумма векторов сторон = 0.

---

[[Dot product of vectors]]
[[Norm of vector]]

**Definition** The *length* ${\|v\|}$ of a vector $v$ is the square root of ${v \cdot v}$:  
$${\text{length} = \|v\| = \sqrt{v \cdot v} = \left(v_1^2 + v_2^2 + \cdots + v_n^2\right)^{1/2}}$$

**Definition** A *unit vector* $u$ is a vector whose length equals one. Then ${u \cdot u = 1}$.

The standard unit vectors along the $x$ and $y$ axes are written $i$ and $j$. In the $xy$ plane, the unit vector that makes an angle “theta” with the $x$ axis is ${(\cos\theta, \sin\theta)}$:  
**Unit vectors** ${i = \left[\begin{matrix}1 \\ 0\end{matrix}\right]}$ and ${j = \left[\begin{matrix}0 \\ 1\end{matrix}\right]}$ and ${u = \left[\begin{matrix}\cos\theta \\ \sin\theta\end{matrix}\right]}$.

**Unit vector** ${u = v / \|v\|}$ is a unit vector in the same direction as $v$.

[[Unit vector]]


![[Pasted image 20260211114249.png]]


**The angle between 2 vectors**
![[dot_product_diagram.svg|400]]

[[Cauchy-Schwarz-Буняковского Inequality]]
SCHWARZ INEQUALITY: ${|v\cdot w|\le \lVert v\rVert \,\lVert w\rVert}$

[[The triangle inequality|Triangle inequality]]
TRIANGLE INEQUALITY: ${\lVert v+w\rVert \le \lVert v\rVert + \lVert w\rVert}$

[[Means]]
[[Expected Value E(X)]]




Матрица разностей

Forward difference (прямая разность)
Backward difference (обратная)
Central difference (центральная)
Cyclic difference
