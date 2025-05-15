---
aliases:
  - Относительная внутренность
anki: false
created: 2024-12-21 19:08
parent:
  - "[[Interior int(S)]]"
connected:
  - "[[Affine hull - aff(S)]]"
tags:
  - empty
---

> [!tip]  Relative Interior of the set $S$
is set:
$\mathbf{relint} (S) = \{\mathbf{x} \in S \mid \exists \varepsilon > 0, \; B(\mathbf{x}, \varepsilon) \cap \mathbf{aff} (S) \subseteq S\}$


#### Difference between interior and relative interior
![[rel_int.svg]]

#### Example
> [!EXAMPLE]
> Any non-empty convex set $S \subseteq \mathbb{R}^n$ has a non-empty relative interior $\mathbf{relint}(S)$.


# Anki
TARGET DECK: Math:: Optimization  
START
Math_ONE_side
TITLE: Relative Interior of the set $S$
DESCRIPTION: is set:
$\mathbf{relint} (S) = \{\mathbf{x} \in S \mid \exists \varepsilon > 0, \; B(\mathbf{x}, \varepsilon) \cap \mathbf{aff} (S) \subseteq S\}$
ADDITIONAL: Example: 
Any non-empty convex set $S \subseteq \mathbb{R}^n$ has a non-empty relative interior $\mathbf{relint}(S)$.
ID: 1734846333074
END

TARGET DECK: Math:: Optimization  
START
Math_ONE_side
TITLE: Difference between interior and relative interior
DESCRIPTION: 
PICTURE: ![[rel_int.svg]]
ID: 1734846333085
END
