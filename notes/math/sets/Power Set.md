---
aliases:
  - Булеан
parent:
  - "[[Set (math)]]"
connected:
  - "[[Subset]]"
  - "[[Cardinality]]"
  - "[[Operations on sets]]"
anki: true
created: 2025-05-20 00:16
tags:
---

> [!tip] Power Set $P(A)$ or $2^A$
> is the set of all [[Subset|subsets]] of set $A$, including empty set $\emptyset$ and $A$ itself

# Properties
For any set $A$: 
- $\emptyset \in P(A)$ and $A \in P(A)$
- If $|A| = n$, then $|P(A)| = 2^n$
- For any sets $A$ and $B$: $A \subseteq B \iff P(A) \subseteq P(B)$
- $P(\emptyset) = \{\emptyset\}$

# Example
For set $A = \{1,2\}$:
$P(A) = \{\emptyset, \{1\}, \{2\}, \{1,2\}\}$

![[Screenshot 2022-07-13 at 12.14.27.png|500]]

# Anki
TARGET DECK: stem::math::sets
START
math_complex
FRONT: Power Set $P(A)$ (def)
BACK: The set of all subsets of set $A$, including empty set and $A$ itself
FORMULA: For set with $n$ elements: $|P(A)| = 2^n$
PICTURE: ![[Screenshot 2022-07-13 at 12.14.27.png]]
ADDITIONAL: Properties:
- $\emptyset \in P(A)$ and $A \in P(A)$
- $A \subseteq B \iff P(A) \subseteq P(B)$
- $P(\emptyset) = \{\emptyset\}$
ID: 1747689641010
END

START
math_basic_single
FRONT: If $|A| = n$, then $|P(A)| = $
BACK: $2^n$
ID: 1747689641019
END

START
math_basic_single
FRONT: Power Set $P(A)$ (prop)
BACK: 1. $\emptyset \in P(A)$ and $A \in P(A)$
2. If $|A| = n$, then $|P(A)| = 2^n$
3. For any sets $A$ and $B$: $A \subseteq B \iff P(A) \subseteq P(B)$
4. $P(\emptyset) = \{\emptyset\}$
ID: 1747689641026
END


