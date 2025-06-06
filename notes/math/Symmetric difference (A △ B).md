---
aliases:
  - Симметричная разность множеств
anki: true
parent:
  - "[[Operations on sets]]"
connected:
  - "[[Difference (A-B)]]"
  - "[[Relative complement]]"
created: 2025-05-15 21:30
tags:
---

> [!tip] Symmetric difference $A \triangle B$ of sets $A$ and $B$
> is the [[Set (math)|set]] that contains all elements of the original sets that do not belong to their intersection.
>$A \triangle B = (A \setminus B) \cup (B \setminus A)$


![[Pasted image 20220712152716.png|500]]

## Properties
- $A \triangle \emptyset = A$
- $A \triangle A = \emptyset$
- $(A\triangle B)\triangle C = A\triangle(B\triangle C) = B\triangle(A\triangle C)$

# Anki
TARGET DECK: stem::math::sets

START
math_complex
FRONT: Symmetric difference $A \triangle B$ (def)
BACK: is the set that contains all elements of the original sets that do not belong to their intersection
FORMULA: $A \triangle B = (A \setminus B) \cup (B \setminus A)$
PICTURE: ![[Pasted image 20220712152716.png]]
ID: 1747335314272
END

START
math_basic_single
FRONT: Symmetric difference (prop)
$A \triangle B =$
BACK: $= (A \setminus B) \cup (B \setminus A)$
ID: 1747344449305
END

START
math_basic_single
FRONT: Symmetric difference (prop)
$A \triangle \emptyset =$
BACK: $A$
ID: 1747344449309
END

START
math_basic_single
FRONT: Symmetric difference (prop)
$A \triangle A =$
BACK: $\emptyset$
ID: 1747344449311
END

START
math_basic_single
FRONT: Symmetric difference (prop)
$(A\triangle B)\triangle C =$
BACK: $A\triangle(B\triangle C) = B\triangle(A\triangle C)$
ID: 1747344449313
END

