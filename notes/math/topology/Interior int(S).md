---
aliases:
  - Внутренность
anki: true
created: 2024-12-21 19:06
parent:
  - "[[515.1 Topology]]"
connected:
  - "[[Open Ball]]"
  - "[[Open set]]"
  - "[[Relative Interior relint(S)]]"
  - "[[Closed set]]"
tags:
  - content/definition
---

> [!tip] Interior of set $S$ denoted $\text{int}(S)$
> is the set of all points in $S$ that have some [[Open Ball|open ball]] entirely contained within $S$.
> $$\text{int}(S) = \{x \in S \mid \exists \varepsilon > 0, \; B(x, \varepsilon) \subset S\}$$
> where $B(x, \varepsilon)$ is the [[Open Ball|open ball]] centered at point $x$ with radius $\varepsilon$.

## Key Properties

- **Interior points**: Every point in $\text{int}(S)$ is surrounded by points of $S$
- **[[Open set|Open]]**: The interior is always an [[Open set|open set]]
- **Subset**: $\text{int}(S) \subseteq S$ always holds
- **Idempotent**: $\text{int}(\text{int}(S)) = \text{int}(S)$
- **Monotone**: If $A \subseteq B$, then $\text{int}(A) \subseteq \text{int}(B)$

## Examples

### In $\mathbb{R}$
- $\text{int}([0,1]) = (0,1)$ - interior of closed interval
- $\text{int}((0,1)) = (0,1)$ - [[Open set|open interval]] equals its interior
- $\text{int}(\{0\}) = \emptyset$ - singleton has empty interior

### In $\mathbb{R}^2$
- $\text{int}(\{(x,y) : x^2 + y^2 \leq 1\}) = \{(x,y) : x^2 + y^2 < 1\}$ - interior of closed disk
- $\text{int}(\{(x,0) : x \in \mathbb{R}\}) = \emptyset$ - line has no interior in plane

## Relationship to [[Open set|Open Sets]]

A set $U$ is [[Open set|open]] if and only if $U = \text{int}(U)$.

![[Relative Interior relint(S)#Difference between interior and relative interior]]

# Anki

TARGET DECK: stem::math::topology
START
math_basic_double
FRONT: Interior of set $S$
BACK: Set of all points in $S$ that have some open ball entirely contained within $S$
ID: 1755935979209
END

TARGET DECK: stem::math::topology
START
math_basic_single
FRONT: Interior vs Open Set
What is the relationship between interior and open sets?
BACK: A set is open if and only if it equals its own interior: $U$ is open $\Leftrightarrow$ $U = \text{int}(U)$
ID: 1755935979210
END

TARGET DECK: stem::math::topology
START
math_complex
FRONT: Interior of Set - Properties
BACK: The interior is the largest open set contained in $S$
FORMULA: $\text{int}(S) = \{x \in S \mid \exists \varepsilon > 0, \; B(x, \varepsilon) \subset S\}$
ADDITIONAL: Properties: always open, idempotent, monotone
ID: 1755935979212
END