---
aliases:
  - Разность множеств
parent:
  - "[[Operations on sets]]"
connected:
  - "[[Symmetric difference (A △ B)]]"
  - "[[Relative complement]]"
anki: true
created: 2025-05-13 18:08
tags:
---

> [!tip] Difference of Sets $A \setminus B$ for sets $A$ and $B$
> is the set of elements that belong to $A$ but not to $B$.
$A \setminus B = \{x \in A | x \notin B\} = A \cap \overline{B}$


![[Pasted image 20220712114121.png|500]]

# Properties
- $A \setminus A = \emptyset$
- $A \setminus \emptyset = A$
- $\emptyset \setminus A = \emptyset$
- $A \setminus \mathbb{U} = \emptyset$
- $\mathbb{U} \setminus A = \overline{A}$
- $A \triangle B = (A \setminus B) \cup (B \setminus A)$ [[Symmetric difference (A △ B)]]

# Anki
TARGET DECK: stem::math::sets

START
math_complex
TITLE: Difference of Sets (def)
$A \setminus B$
DESCRIPTION: is the set of elements that belong to $A$ but not to $B$.
FORMULA: $A \setminus B = \{x \in A | x \notin B\} = A \cap \overline{B}$
PICTURE: ![[Pasted image 20220712114121.png]]
ID: 1747383865728
END

START
math_basic_double
FRONT: Difference of Sets (prop)
$A \setminus B =$
BACK: $= \{x \in A | x \notin B\} = A \cap \overline{B}$
ID: 1747383899365
END

START
math_basic_single
FRONT: Difference of Sets (prop)
$A \setminus A =$
BACK: $= \emptyset$
ID: 1747383865738
END

START
math_basic_single
FRONT: Difference of Sets (prop)
$A \setminus \emptyset =$
BACK: $= A$
ID: 1747383865742
END

START
math_basic_single
FRONT: Difference of Sets (prop)
$\emptyset \setminus A =$
BACK: $= \emptyset$
ID: 1747383865745
END

START
math_basic_single
FRONT: Difference of Sets (prop)
$A \setminus \mathbb{U} =$
BACK: $= \emptyset$
ID: 1747383865748
END

START
math_basic_single
FRONT: Difference of Sets (prop)
$\mathbb{U} \setminus A =$
BACK: $= \overline{A}$
ID: 1747383865752
END

START
math_basic_single
FRONT: Difference of Sets (prop)
$A \triangle B =$
BACK: $= (A \setminus B) \cup (B \setminus A)$
ID: 1747383865755
END



