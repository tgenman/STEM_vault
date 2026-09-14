---
aliases:
  - Равномощность множеств
  - Equinumerous sets
  - Cardinality equivalence of sets
parent:
  - "[[Binary relation]]"
  - "[[Cardinality]]"
  - "[[Bijective mapping property (function)]]"
connected:
  - "[[Countable set]]"
  - "[[Infinity set]]"
created: 2025-05-20 10:41
anki: true
tags:
---

> [!tip] Equipotent Sets (Sets of Equal Cardinality)
> Two sets $A$ and $B$ are equipotent (have the same cardinality) if and only if there exists a [[Bijective mapping property (function)|bijective function]] $f : A \rightarrow B$

This is denoted as $A \sim B$ or $|A| = |B|$

# Properties
1. [[Reflexive]] : $A \sim A$ for any set $A$
2. [[Symmetry]]: If $A \sim B$, then $B \sim A$
3. [[Transitive]] : If $A \sim B$ and $B \sim C$, then $A \sim C$

# Examples
1. Sets $\mathbb{N}$ and $\mathbb{Z}$ are equipotent
2. Sets $[0,1]$ and $(0,1)$ are equipotent
3. Sets with the same finite number of elements are equipotent

# Anki
TARGET DECK: stem::math::sets

START
math_complex
FRONT: Equipotent Sets (Sets of Equal Cardinality)
BACK: Two sets $A$ and $B$ are equipotent if there exists a bijective function between them
FORMULA: $A \sim B \iff \exists f: A \rightarrow B$ (bijective)
ADDITIONAL: Properties:
- Reflexivity: $A \sim A$
- Symmetry: If $A \sim B$, then $B \sim A$
- Transitivity: If $A \sim B$ and $B \sim C$, then $A \sim C$
ID: 1747727528279
END

START
math_basic_single
FRONT: Sets $A$ and $B$ that have a bijective function $f : A \rightarrow B$ between them. Name sets
BACK: Equipotent Sets
ID: 1747727528287
END