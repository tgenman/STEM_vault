---
aliases:
  - Подмножество
anki: true
created: 2023-10-17 17:39
parent:
  - "[[Set (math)]]"
connected:
  - "[[Empty Set]]"
  - "[[Improper subset]]"
  - "[[Proper subset]]"
---

> [!tip] A set $B$ is a subset of a set $A$ (denoted by $B⊆A$ or $A⊇B$), 
> if every element of $B$ is in $A$. 
> The notations $B ⊂ A$ or $A ⊃ B$ will be used for $B ⊆ A$ but $B  \neq A$.


# Properties of Subsets
- **Reflexivity** 
    - $A⊆A$
- **Transitivity**
    - If $B⊆A$ and $A⊆K$, then $B⊆K$
- **Antisymmetry**
    - If $A⊆B$ and $B⊆A$, then $A=B$
- For any set $A$, $A$ itself and $∅$ are both subsets of $A$

# Anki
TARGET DECK: stem::math::sets
START
math_basic_single
QUESTION: What is a subset? ($B⊆A$ or $A⊇B$)
ANSWER: A set $B$ is a subset of set $A$ if every element of $B$ is in $A$
ID: 1747686174306
END

START
math_basic_single
QUESTION: Difference between $B ⊂ A$ and $B ⊆ A$
ANSWER: $B ⊂ A$ means $B ⊆ A$ but $B \neq A$ (strict subset)
ID: 1747686174310
END

START
math_basic_complex
TITLE: Properties of Subsets
DESCRIPTION: For sets $A$, $B$, and $K$:
1. Reflexivity: $A ⊆ A$
2. Transitivity: If $B ⊆ A$ and $A ⊆ K$, then $B ⊆ K$
3. Antisymmetry: If $A ⊆ B$ and $B ⊆ A$, then $A = B$
4. Universal subsets: For any set $A$, both $A$ and $∅$ are subsets of $A$
ADDITIONAL: These properties form the foundation for partial ordering in set theory
END


