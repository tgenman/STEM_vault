---
aliases:
  - Декартово произведение множеств
anki: true
parent:
  - "[[Operations on sets]]"
created: 2023-10-17 18:18
connected:
  - "[[Tuple]]"
---

> [!tip] Cartesian product of $A$ and $B$.
The set $A×B=\set{(a,b)|a∈A\text{ and }b∈B}$


> [!tip]  Product rule
The [[Cardinality]] of a Cartesian product of sets equals the product of the cardinalities of these sets
$$|A \times B | = |A| \cdot |B|$$

### Properties
1. $(A_1 \cup A_2) \times B = (A_1 \times B) \cup (A_2 \times B)$
2. $A \times (B_1 \cup B_2) = (A \times B_1) \cup (A \times B_2)$
3. $(A_1 \cap A_2) \times B = (A_1 \times B) \cap (A_2 \times B)$
4. $A \times (B_1 \cap B_2) = (A \times B_1) \cap (A \times B_2)$
5. $(A_1 \setminus A_2) \times B = (A_1 \times B) \setminus (A_2 \times B)$
6. $A \times (B_1 \setminus B_2) = (A \times B_1) \setminus (A \times B_2)$


# Anki
TARGET DECK: stem::math::sets
START
math_basic_single
FRONT: Cartesian product of sets (def).
BACK: The set $A×B=\set{(a,b)|a∈A\text{ and }b∈B}$
ID: 1747685141979
END

START
math_basic_single
FRONT: The [[Cardinality]] of a Cartesian product of sets equals
BACK: the product of the cardinalities of these sets
$|A \times B | = |A| \cdot |B|$
ID: 1747685007756
END

START
math_basic_single
FRONT: Cartesian product (prop)
$(A_1 \cup A_2) \times B =$
BACK: $= (A_1 \times B) \cup (A_2 \times B)$
ID: 1747684797507
END

START
math_basic_single
FRONT: Cartesian product (prop)
$A \times (B_1 \cup B_2) =$
BACK: $= (A \times B_1) \cup (A \times B_2)$
ID: 1747684797511
END

START
math_basic_single
FRONT: Cartesian product (prop)
$(A_1 \cap A_2) \times B =$
BACK: $= (A_1 \times B) \cap (A_2 \times B)$
ID: 1747684797514
END

START
math_basic_single
FRONT: Cartesian product (prop)
$A \times (B_1 \cap B_2) =$
BACK: $= (A \times B_1) \cap (A \times B_2)$
ID: 1747684797517
END

START
math_basic_single
FRONT: Cartesian product (prop)
$(A_1 \setminus A_2) \times B =$
BACK: $= (A_1 \times B) \setminus (A_2 \times B)$
ID: 1747684797519
END

START
math_basic_single
FRONT: Cartesian product (prop)
$A \times (B_1 \setminus B_2) =$
BACK: $= (A \times B_1) \setminus (A \times B_2)$
ID: 1747684797522
END