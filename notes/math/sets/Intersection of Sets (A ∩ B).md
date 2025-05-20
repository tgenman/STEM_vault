---
aliases:
  - Пересечение множеств
parent:
  - "[[Operations on sets]]"
connected:
  - "[[Logical AND (∧)]]"
  - "[[Venn-Euler diagram]]"
  - "[[Properties of intersection and union]]"
anki: true
created: 2025-05-20 10:12
tags: 
---

> [!tip] Intersection of Sets $A \cap B$ for sets $A$ and $B$
> is the set of all elements that belong to both sets simultaneously.
$A \cap B = \{x \mid x \in A \text{ and } x \in B\}$

![[Pasted image 20220630190715.png]]

# Properties
- [[Commutative identity|Commutativity]] : $A \cap B = B \cap A$
- [[Associative identity|Associativity]] : $(A \cap B) \cap C = A \cap (B \cap C)$
- Empty set: $A \cap \emptyset = \emptyset$
- [[Idempotence]]: $A \cap A = A$
- Subset property: If $A \subseteq B$, then $A \cap B = A$

# Anki
TARGET DECK: stem::math::sets
START
math_basic_double
FRONT: Intersection of Sets (def)
$A \cap B =$
BACK: The set of all elements that belong to both sets $A$ and $B$ simultaneously
$= \{x \mid x \in A \text{ and } x \in B\}$
ID: 1747725553589
END

START
math_basic_single
FRONT: Intersection of Sets (prop)
What is $A \cap \emptyset$?
BACK: $\emptyset$ (empty set)
ID: 1747725553593
END

START
math_complex
FRONT: Intersection of Sets
BACK: The set of all elements that belong to both sets simultaneously
FORMULA: $A \cap B = \{x \mid x \in A \text{ and } x \in B\}$
PICTURE: ![[Pasted image 20220630190715.png]]
ADDITIONAL: Properties:
- Commutativity: $A \cap B = B \cap A$
- Associativity: $(A \cap B) \cap C = A \cap (B \cap C)$
- Empty set: $A \cap \emptyset = \emptyset$
- Idempotence: $A \cap A = A$
- Subset property: If $A \subseteq B$, then $A \cap B = A$
ID: 1747725553596
END