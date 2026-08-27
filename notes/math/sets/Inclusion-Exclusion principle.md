---
aliases:
  - Формула включений-исключений
anki: true
created: 2023-10-20 21:01
parent:
  - "[[510.22 Set theory]]"
connected:
  - "[[519.21  Probability theory|Probability theory]]"
  - "[[Cardinality]]"
  - "[[519.101 Combinatorics MOC]]"
  - "[[Union of Sets (A U B)]]"
  - "[[Operations on sets]]"
  - "[[Intersection]]"
tags:
---

> [!tip] Inclusion-Exclusion Principle
> is a counting technique that computes the cardinality of a union of multiple sets by adding the cardinalities of the individual sets, then subtracting the cardinalities of their pairwise intersections, then adding the cardinalities of their triple-wise intersections, and so on, with alternating signs.
$P(A_1 \cup \ldots \cup A_k) = P(A_1) + \ldots + P(A_n) -$
$- P(A_1 \cap A_2) - P(A_1 \cap A_3) - \ldots - P(A_{k-1} \cap A_k) + \ldots + (-1)^{k-1}P(A_1 \cap \ldots \cap A_k)$

$|A_1 \cup A_2 \cup \ldots \cup A_n| = \sum_{S \neq \emptyset} (-1)^{|S|+1} \left| \bigcap_{i \in S} A_i \right|$

## Special Cases

### For two sets
$$|A \cup B| = |A| + |B| - |A \cap B|$$

### For three sets
$$|A \cup B \cup C| = |A| + |B| + |C| - |A \cap B| - |A \cap C| - |B \cap C| + |A \cap B \cap C|$$

![[Pasted image 20231020210108.png|300]]

## Probability Form

For events $A_1, A_2, \ldots, A_n$ in a probability space, the probability of their union is:

$$P(A_1 \cup A_2 \cup \ldots \cup A_n) = \sum_{i=1}^{n} P(A_i) - \sum_{1 \leq i < j \leq n} P(A_i \cap A_j) + \sum_{1 \leq i < j < k \leq n} P(A_i \cap A_j \cap A_k) - \ldots + (-1)^{n+1} P(A_1 \cap A_2 \cap \ldots \cap A_n)$$

# Anki
TARGET DECK: stem::math::sets
S
TART
math_complex
FRONT: Inclusion-Exclusion Principle
BACK: A counting technique that computes the cardinality of a union of multiple sets by adding the cardinalities of individual sets, then subtracting the cardinalities of pairwise intersections, then adding triple-wise intersections, and so on with alternating signs.
FORMULA: $$|A_1 \cup A_2 \cup \ldots \cup A_n| = \sum_{i=1}^{n} |A_i| - \sum_{1 \leq i < j \leq n} |A_i \cap A_j| + \sum_{1 \leq i < j < k \leq n} |A_i \cap A_j \cap A_k| - \ldots + (-1)^{n+1} |A_1 \cap A_2 \cap \ldots \cap A_n|$$
PICTURE: ![[Pasted image 20231020210108.png]]
ADDITIONAL: Special cases:
- For 2 sets: |A ∪ B| = |A| + |B| - |A ∩ B|
- For 3 sets: |A ∪ B ∪ C| = |A| + |B| + |C| - |A ∩ B| - |A ∩ C| - |B ∩ C| + |A ∩ B ∩ C|
- Has probability form: P(A₁ ∪ ... ∪ Aₙ) with same structure
END

START
math_basic_single
FRONT: What is the formula for the union of two sets using the Inclusion-Exclusion Principle?
BACK: $|A \cup B| = |A| + |B| - |A \cap B|$
ID: 1747852031279
END

START
math_basic_single
FRONT: What is the formula for the union of three sets using the Inclusion-Exclusion Principle?
BACK: $|A \cup B \cup C| = |A| + |B| + |C| - |A \cap B| - |A \cap C| - |B \cap C| + |A \cap B \cap C|$
ID: 1747852031281
END

START
math_basic_double
FRONT: Inclusion-Exclusion Principle
BACK: A counting technique for computing the cardinality of a union of sets using alternating sums of intersection cardinalities
ID: 1747852031283
END

