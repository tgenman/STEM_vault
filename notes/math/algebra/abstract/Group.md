---
aliases:
  - Группа
anki: false
created: 2023-10-21 13:11
parent:
  - "[[Monoid]]"
  - "[[Algebraic Structure]]"
connected:
  - "[[Abelian group]]"
  - "[[512.5 General Algebra MOC]]"
tags:
  - empty
---
Это [[Monoid]] c наличием [[Inverse element]]


> [!tip] Group
Consider a set $\mathcal{G}$ and an operation $\otimes : \mathcal{G} \times \mathcal{G} \to \mathcal{G}$ defined on $\mathcal{G}$. 
Then $\mathcal{G} := (\mathcal{G}, \otimes)$ is called a group if the following hold:
1. *Closure of $\mathcal{G}$ under $\otimes$*: $\forall x, y \in \mathcal{G} : x \otimes y \in \mathcal{G}$
2. *Associativity*: $\forall x, y, z \in \mathcal{G} : (x \otimes y) \otimes z = x \otimes (y \otimes z)$
3. *Neutral element* [[Identity element]] : $\exists e \in \mathcal{G} \forall x \in \mathcal{G} : x \otimes e = x$ and $e \otimes x = x$
4. [[Inverse element]]: $\forall x \in \mathcal{G} \exists y \in \mathcal{G} : x \otimes y = e$ and $y \otimes x = e$, where $e$ is the neutral element. We often write $x^{-1}$ to denote the inverse element of $x$.



If additionally $\forall x, y \in \mathcal{G} : x \otimes y = y \otimes x$, then $\mathcal{G} = (\mathcal{G}, \otimes)$ is an *Abelian group* (commutative).










