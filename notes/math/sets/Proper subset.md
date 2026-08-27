---
aliases:
  - Собственное подмножество
anki: true
created: 2023-10-17 18:30
parent:
  - "[[Subset]]"
connected:
  - "[[Improper subset]]"
---

> [!tip] Proper subset $A \subset B$
> is a subset of set $B$ that is not equal to $B$ itself and is not an [[Empty Set|empty set]] $\emptyset$

# Properties
- If $A$ is a proper subset of $B$, then $|A| < |B|$
- For any non-empty set $B$, there exists at least one proper subset
- The relation of proper subset is transitive: if $A \subset B$ and $B \subset C$, then $A \subset C$

# Anki
TARGET DECK: stem::math::sets
START
math_complex
FRONT: Proper subset $A \subset B$ (def)
BACK: A subset of a set that excludes two cases: the set itself and the empty set
ADDITIONAL: If $A$ is a proper subset of $B$, then:
$A \subset B$ and $A \neq B$ and $A \neq \emptyset$
ID: 1747687634584
END

START
math_basic_single
FRONT: Proper subset $A \subset B$ (prop)
BACK: 
1) $|A| < |B|$
2) Any non-empty set $B$ has at least one proper subset
3) Transitivity: if $A \subset B$ and $B \subset C$, then $A \subset C$
ID: 1747687634591
END












