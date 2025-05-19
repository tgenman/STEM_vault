---
aliases:
  - Мощность множества
  - Cardinal number
anki: true
created: 2023-10-17 21:05
parent:
  - "[[Set (math)]]"
connected:
  - "[[The bijection rule]]"
  - "[[Countable infinity set]]"
  - "[[Continuum infinity set]]"
  - "[[Правило суммы мощностей множеств]]"
  - "[[Inclusion-Exclusion principle]]"
  - "[[Cartesian product of sets]]"
tags:
---

> [!tip] Cardinality $|X|$ of a set $X$
> is the number of elements in the set.

For finite sets, cardinality is simply the count of elements. For infinite sets, we use [[The bijection rule]] to compare their sizes.

# Properties
1. Empty set has cardinality zero: $|\emptyset| = 0$
2. For [[Disjoint set|disjoint sets]] $A$ and $B$: $|A \cup B| = |A| + |B|$ ([[Правило суммы мощностей множеств]])
3. For any sets $A$ and $B$: $|A \cup B| = |A| + |B| - |A \cap B|$ ([[Inclusion-Exclusion principle]])
4. For [[Cartesian product of sets|Cartesian product]]: $|A \times B| = |A| \cdot |B|$

# Types of Infinite Cardinality
1. [[Countable infinity set|Countable]] (denoted as $\aleph_0$)
   - Examples: $|\mathbb{N}| = |\mathbb{Z}| = |\mathbb{Q}| = \aleph_0$
2. [[Continuum infinity set|Uncountable]] (denoted as $\mathfrak{c}$ or $2^{\aleph_0}$)
   - Examples: $|\mathbb{R}| = |\mathbb{C}| = \mathfrak{c}$

# Anki
TARGET DECK: stem::math::sets
START
math_complex
FRONT: Cardinality
BACK: The number of elements in a set $X$, denoted as $|X|$
FORMULA: 
For disjoint sets: $|A \cup B| = |A| + |B|$
For any sets: $|A \cup B| = |A| + |B| - |A \cap B|$
For Cartesian product: $|A \times B| = |A| \cdot |B|$
ADDITIONAL: Types:
- Finite cardinality: counting elements
- Countable infinity ($\aleph_0$): e.g., $|\mathbb{N}|$
- Uncountable infinity ($\mathfrak{c}$): e.g., $|\mathbb{R}|$
ID: 1747688508469
END

START
math_basic_single
FRONT: What is the cardinality of empty set?
BACK: $|\emptyset| = 0$
ID: 1747688508473
END









 


