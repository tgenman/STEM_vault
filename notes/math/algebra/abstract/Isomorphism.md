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
TARGET DECK: stem::math::algebra

START
math_complex
TITLE: Isomorphism
DESCRIPTION: A [[Homomorphism|homomorphism]] that is also [[Bijective mapping property (function)|bijective]]. Each element in one structure corresponds to exactly one element in another, preserving all operations.
FORMULA: For operation $\ast$ in $A$ and $\circ$ in $B$: $\phi(x \ast y) = \phi(x) \circ \phi(y)$ where $\phi$ is bijective
ADDITIONAL:
ID: 1747395543806
END

START
math_complex
TITLE: Isomorphism Properties
DESCRIPTION: Key characteristics of isomorphisms between algebraic structures
- [[Inverse function (math)|Invertible]]: An inverse isomorphism exists
- Structure-preserving: Completely preserves structural operations
- [[Bijective mapping property (function)|Bijective]]: One-to-one correspondence between elements
ADDITIONAL:
ID: 1747395543810
END


















