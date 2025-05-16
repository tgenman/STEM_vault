---
aliases:
  - Гомоморфизм
anki: true
created: 2024-01-08 13:35
parent:
  - "[[512.5 General Algebra MOC]]"
connected:
  - "[[Isomorphism]]"
  - "[[Algebraic Structure]]"
  - "[[Group]]"
  - "[[Ring]]"
  - "[[Field]]"
  - "[[Kernel]]"
---

> [!tip] Homomorphism
> A function $\phi: A \to B$ between two [[Algebraic Structure|algebraic structures]] (e.g., [[Group|groups]], [[Ring|rings]], [[Field|fields]]) that preserves the structure operations. For any operation $\ast$ in $A$ and corresponding operation $\circ$ in $B$, the relationship $\phi(x \ast y) = \phi(x) \circ \phi(y)$ holds.

# Properties
- Preserves [[Algebraic Structure|algebraic structure]] operations
- Not necessarily [[Bijective mapping property (function)|bijective]]  or invertible
- May map different elements of source structure to the same element in target structure
- [[Kernel|Kernel]] of a homomorphism: set of elements mapped to the identity element
- Forms the fundamental concept for studying structure relationships

# Examples
## Group Homomorphism
For [[Group|groups]] $(G, \ast)$ and $(H, \circ)$, a function $\phi: G \to H$ is a homomorphism if:
$\phi(a \ast b) = \phi(a) \circ \phi(b)$ for all $a, b \in G$.

## Ring Homomorphism
For [[Ring|rings]] $(R, +, \cdot)$ and $(S, \oplus, \otimes)$, a function $\phi: R \to S$ is a homomorphism if:
- $\phi(a + b) = \phi(a) \oplus \phi(b)$
- $\phi(a \cdot b) = \phi(a) \otimes \phi(b)$
for all $a, b \in R$.

# Related Concepts
- A [[Isomorphism|isomorphism]] is a bijective homomorphism
- The [[Kernel|kernel]] of a homomorphism is a normal subgroup (in group theory)
- The [[Range Ran(f) or Image Im(f)|image]] of a homomorphism is a substructure of the target structure

# Anki
TARGET DECK: stem::math::algebra 

START
math_complex
TITLE: Homomorphism
DESCRIPTION: A function $\phi: A \to B$ between two [[Algebraic Structure|algebraic structures]] (e.g., [[Group|groups]], [[Ring|rings]], [[Field|fields]]) that preserves the structure operations. For any operation $\ast$ in $A$ and corresponding operation $\circ$ in $B$, the relationship $\phi(x \ast y) = \phi(x) \circ \phi(y)$ holds.
FORMULA: For groups: $\phi(a \ast b) = \phi(a) \circ \phi(b)$
For rings: $\phi(a + b) = \phi(a) \oplus \phi(b)$ and $\phi(a \cdot b) = \phi(a) \otimes \phi(b)$
ADDITIONAL:
ID: 1747395478834
END

START
math_complex
TITLE: Homomorphism Properties
DESCRIPTION: Key properties of homomorphisms between algebraic structures
- Preserves algebraic structure operations
- Not necessarily bijective or invertible
- May map different elements of source structure to the same element in target structure
- Has a [[Kernel|kernel]]: set of elements mapped to the identity element
- Forms the fundamental concept for studying structure relationships
ADDITIONAL:
ID: 1747395478838
END





