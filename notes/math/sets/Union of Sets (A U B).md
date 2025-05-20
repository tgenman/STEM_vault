---
aliases:
  - Объединение множеств
anki: true
parent:
  - "[[Operations on sets]]"
connected:
  - "[[Properties of intersection and union]]"
  - "[[Venn-Euler diagram]]"
created: 2024-03-24 16:47
anki: true
tags:
---

> [!tip] Union of Sets $A \cup B$
> is a set that contains all elements that belong to either set $A$ or set $B$ (or both).
$A \cup B = \{x \mid x \in A \text{ or } x \in B\}$

![[Pasted image 20220630193329.png]]

# Properties
- [[Commutative identity|Commutativity]] : $A \cup B = B \cup A$
- [[Associative identity|Associativity]] : $(A \cup B) \cup C = A \cup (B \cup C)$
- Identity: $A \cup \emptyset = A$
- [[Idempotence]]: $A \cup A = A$

# Anki
TARGET DECK: stem::math::sets
START
math_basic_double
FRONT: Union of Sets $A \cup B$
BACK: A set containing all elements that belong to either set $A$ or set $B$ (or both).
$A \cup B = \{x \mid x \in A \text{ or } x \in B\}$
ID: 1747726318105
END

START
math_basic_single
FRONT: Union with empty set
$A \cup \emptyset =$
BACK: $= A$
ID: 1747726318109
END

START
math_complex
FRONT: Union of Sets
BACK: A fundamental set operation that combines elements from two sets
FORMULA: $A \cup B = \{x \mid x \in A \text{ or } x \in B\}$
PICTURE: ![[Pasted image 20220630193329.png]]
ADDITIONAL: Properties:
- Commutative: $A \cup B = B \cup A$
- Associative: $(A \cup B) \cup C = A \cup (B \cup C)$
- Identity: $A \cup \emptyset = A$
- Idempotent: $A \cup A = A$
ID: 1747726318112
END