---
aliases:
  - Изоморфизм
anki: true
created: 2024-01-08 13:35
parent:
  - "[[512.5 General Algebra MOC]]"
connected:
  - "[[Homomorphism]]"
  - "[[Bijective mapping property (function)]]"
  - "[[Algebraic Structure]]"
  - "[[519.175.1 Isomorphic Graphs]]"
---

> [!tip] Isomorphism
> A [[Homomorphism|homomorphism]] that is also a [[Bijective mapping property (function)|bijective function]], meaning it is both one-to-one and onto. This establishes that each element in one structure corresponds to exactly one element in another structure, and vice versa.

# Properties
- [[Inverse function (math)|Invertible]]: An inverse isomorphism exists
- **Structure-preserving**: Completely preserves the structure, indicating that the structures are essentially identical
- [[Bijective mapping property (function)|bijective]]: Provides a one-to-one correspondence between elements of both structures

# Applications
Used to demonstrate that two structures are not merely similar but "identical" in an algebraic sense, differing only in the "labels" assigned to their elements.

# Relation to Homomorphisms
All isomorphisms are homomorphisms, but not all homomorphisms are isomorphisms. An isomorphism indicates a deeper similarity between structures than a homomorphism.

# Examples
## Group Isomorphism
For [[Group|groups]] $(G, \ast)$ and $(H, \circ)$, a bijective function $\phi: G \to H$ is an isomorphism if:
$\phi(a \ast b) = \phi(a) \circ \phi(b)$ for all $a, b \in G$.

## Ring Isomorphism
For [[Ring|rings]] $(R, +, \cdot)$ and $(S, \oplus, \otimes)$, a bijective function $\phi: R \to S$ is an isomorphism if:
- $\phi(a + b) = \phi(a) \oplus \phi(b)$
- $\phi(a \cdot b) = \phi(a) \otimes \phi(b)$
for all $a, b \in R$.

# Anki
> [!question]- Isomorphism
TARGET DECK: stem::math::algebra
START
Math_TWO_side
TITLE: Isomorphism
DESCRIPTION: A [[Homomorphism|homomorphism]] that is also [[Bijective mapping property (function)|bijective]]. Each element in one structure corresponds to exactly one element in another, preserving all operations.
FORMULA: For operation $\ast$ in $A$ and $\circ$ in $B$: $\phi(x \ast y) = \phi(x) \circ \phi(y)$ where $\phi$ is bijective
ADDITIONAL:
ID: 1746385786412
END

> [!question]- Isomorphism Properties
START
Math_TWO_side
TITLE: Isomorphism Properties
DESCRIPTION: Key characteristics of isomorphisms between algebraic structures
- [[Inverse function (math)|Invertible]]: An inverse isomorphism exists
- Structure-preserving: Completely preserves structural operations
- [[Bijective mapping property (function)|Bijective]]: One-to-one correspondence between elements
ADDITIONAL:
ID: 1746385673146
END


> [!question]- Group Isomorphism
START
Math_TWO_side
TITLE: Group Isomorphism
DESCRIPTION: A bijective homomorphism between two [[Group|groups]] that preserves the group operation.
FORMULA: For groups $(G, \ast)$ and $(H, \circ)$, a bijective function $\phi: G \to H$ is an isomorphism if:
$\phi(a \ast b) = \phi(a) \circ \phi(b)$ for all $a, b \in G$
ADDITIONAL:
ID: 1746385673150
END

> [!question]- Ring Isomorphism
START
Math_TWO_side
TITLE: Ring Isomorphism
DESCRIPTION: A bijective homomorphism between two [[Ring|rings]] that preserves both ring operations (addition and multiplication).
FORMULA: For rings $(R, +, \cdot)$ and $(S, \oplus, \otimes)$, a bijective function $\phi: R \to S$ is an isomorphism if:
$\phi(a + b) = \phi(a) \oplus \phi(b)$ and
$\phi(a \cdot b) = \phi(a) \otimes \phi(b)$ for all $a, b \in R$
ADDITIONAL:
ID: 1746385673153
END





















