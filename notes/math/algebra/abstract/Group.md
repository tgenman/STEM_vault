---
aliases:
  - Группа
anki: true
created: 2023-10-21 13:11
parent:
  - "[[Monoid]]"
  - "[[Algebraic Structure]]"
connected:
  - "[[Abelian group]]"
  - "[[512.5 General Algebra MOC]]"
tags:
---

> [!tip] Group (formal definition)
> A group is a set $G$ with a [[Binary operation|binary operation]] $*$ satisfying:
> - [[Closure of]] $G$: $\forall a,b \in G: a * b \in G$
> - [[Associative identity]]: $\forall a,b,c \in G: (a * b) * c = a * (b * c)$
> - [[Identity element]]: $\exists e \in G \forall g \in G: e * g = g * e = g$
> - [[Inverse element]]: $\forall g \in G \exists g^{-1} \in G: g * g^{-1} = g^{-1} * g = e$

> [!tip] Group (definition 2)
> is a [[Monoid]] with the presence of an [[Inverse element]]

If additionally [[Commutative identity]] $\forall x, y \in \mathcal{G} : x \otimes y = y \otimes x$, then $\mathcal{G} = (\mathcal{G}, \otimes)$ is an [[Abelian group]].

**Remarks**  
- We frequently omit the symbol and write, e.g., $xy$ for $x * y$.
- We only use $+$ if $G$ is abelian. Thus, $g + h = h + g$ (always), but in general, $gh \neq hg$.

# Anki
TARGET DECK: stem::math::algebra
START
Math_ONE_side
TITLE: Group (formal definition)
DESCRIPTION: A set $G$ with a binary operation $*$ satisfying:
> - Closure: $\forall a,b \in G: a * b \in G$
> - Associativity: $\forall a,b,c \in G: (a * b) * c = a * (b * c)$
> - Identity: $\exists e \in G \forall g \in G: e * g = g * e = g$
> - Inverses: $\forall g \in G \exists g^{-1} \in G: g * g^{-1} = g^{-1} * g = e$
FORMULA: 
ADDITIONAL:
ID: 1746886388944
END

TARGET DECK: stem::math::algebra
START
Math_ONE_side
TITLE: Group (alternative definition)
DESCRIPTION: is a monoid with the presence of an inverse element
FORMULA: 
ADDITIONAL:
ID: 1746886388949
END





