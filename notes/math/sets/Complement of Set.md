---
aliases:
  - Дополнение множества
anki: true
parent:
  - "[[Operations on sets]]"
connected:
  - "[[Complement of a Graph]]"
  - "[[Universal set]]"
  - "[[Empty set]]"
created: 2025-05-20 00:22
tags:
---

> [!tip] Complement of set $A$ (or its negation) $\overline{A}$, $A^c$, or $A'$
> is a [[Set (math)|set]] that consists of all elements that do not belong to $A$ (within the universal set $U$)

![[Pasted image 20220712111557.png|500]]

# Properties
1. **Universal Property**: $A \cup \overline{A} = U$
2. **Empty Intersection**: $A \cap \overline{A} = \emptyset$
3. **Universal Set Complement**: $\overline{U} = \emptyset$
4. **Double Complement**: $\bar{\bar{A}} = A$
5. [[De Morgan's laws]]
   - $\overline{A \cup B} = \overline{A} \cap \overline{B}$
   - $\overline{A \cap B} = \overline{A} \cup \overline{B}$

# Examples
- If $U = \{1,2,3,4,5\}$ and $A = \{1,2,3\}$, then $\overline{A} = \{4,5\}$
- If $U = \mathbb{R}$ and $A = [0,1]$, then $\overline{A} = (-\infty,0) \cup (1,\infty)$

# Anki
TARGET DECK: stem::math::sets
START
math_basic_double
FRONT: Complement of Set $\overline{A}$ (def)
BACK: Set of all elements in universal set $U$ that do not belong to $A$
![[Pasted image 20220712111557.png]]
ID: 1747690187380
END

START
math_basic_single
FRONT: For complement of set (prop):
$A \cup \overline{A} =$
BACK: $= U$
ID: 1747690187383
END

START
math_basic_single
FRONT: For complement of set (prop):
$A \cap \overline{A} =$
BACK: $= \emptyset$
ID: 1747690187386
END

START
math_basic_single
FRONT: For complement of set (prop):
$\overline{U} =$
BACK: $= \emptyset$
ID: 1747690187388
END

START
math_basic_single
FRONT: For complement of set (prop):
$\bar{\bar{A}} =$
BACK: $= A$
ID: 1747690187390
END



