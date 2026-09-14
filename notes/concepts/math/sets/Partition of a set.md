---
aliases:
  - Разбиение множества
anki: true
created: 2023-10-21 17:16
parent:
  - "[[Operations on sets]]"
connected:
  - "[[Disjoint set]]"
  - "[[Set (math)]]"
  - "[[Empty Set]]"
---

> [!tip] A partition of a set $S$
> is a collection $\{A_i\}_{i \in I}$ of nonempty [[Disjoint set|disjoint]] [[Subset|subsets]] of $S$ such that their union equals $S$:
> 1. $A_i \cap A_j = \emptyset$ for all $i \neq j$ (disjointness)
> 2. $\bigcup_{i \in I} A_i = S$ (completeness)
> 3. $A_i \neq \emptyset$ for all $i \in I$ (non-emptiness)

The subsets $A_i$ are called the ==blocks== or ==cells== of the partition.

# Properties
- Every non-[[Empty Set|empty set]] has at least one partition (the trivial partition consisting of the set itself)
- The number of different ways to partition a set with $n$ elements is called the [[Bell numbers]] $B_n$
- For any partition $\{A_i\}_{i \in I}$ of $S$:
    - $|S| = \sum_{i \in I} |A_i|$ (by [[Sum Rule for Set Cardinalities|sum rule for cardinalities]])

# Anki
TARGET DECK: stem::math::sets
START
math_complex
FRONT: Partition of a set $S$ (def)
BACK: A collection $\{A_i\}_{i \in I}$ of nonempty disjoint subsets of $S$ such that:
1. $A_i \cap A_j = \emptyset$ for all $i \neq j$ (disjointness)
2. $\bigcup_{i \in I} A_i = S$ (completeness)
3. $A_i \neq \emptyset$ for all $i \in I$ (non-emptiness)
ADDITIONAL: The subsets $A_i$ are called blocks or cells of the partition
ID: 1747689306648
END

START
math_basic_single
FRONT: For a partition $\{A_i\}_{i \in I}$ of set $S$, what is $|S|$?
BACK: $|S| = \sum_{i \in I} |A_i|$
ID: 1747689306652
END

START
math_basic_single
FRONT: What is the minimum number of partitions for a non-empty set?
BACK: At least one (the trivial partition consisting of the set itself)
ID: 1747689306655
END




