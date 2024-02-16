---
aliases:
  - Классическое определение вероятности
publish: true
anki: true
created: 2023-10-20 20:39
parent:
  - "[[Probability]]"
connected: []
---
### Classical definition of probability 
$\Omega = \{\omega_1, ..., \omega_n\}$ - [[Sample space]] of [[Elementary event]]s
$A \subset \Omega$ - [[Event]]
$P(A) = \frac{|A|}{n}$ - [[Probability]]

### Probability Properties
- Axioms
	- Normalization $P(\Omega) = 1$
	- Nonnegativity $P(A) >= 0$
	- Additivity $P(A \sqcup B ) = P(A) + P(B)$ - $A, B$ are disjoint sets
- $𝑃 (𝐴) = 0 ⇔ 𝐴 = ∅$ - только [[Empty Set]]  имеет нулевую вероятность
- $𝑃 (𝐴 ∪ 𝐵) = 𝑃(𝐴)+𝑃(𝐵)−𝑃(𝐴∩𝐵)$ - для произвольных событий
	- [[Inclusion-Exclusion principle]]
- $P(A,\cup...\cup A_k)\leq P(A_1)+...+P(A_k)$
- $\bar{A}:=\Omega\backslash A\text{ paвна }P(\bar{A})=1-P(A)$


### Anki
> [!question]-
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Classical definition of probability
DESCRIPTION: $\Omega = \{\omega_1, ..., \omega_n\}$ - [[Sample space]] of [[Elementary event]]s
$A \subset \Omega$ - [[Event]]
$P(A) = \frac{|A|}{n}$ - [[Probability]]
ID: 1697972721265
END

> [!question]-
START
Math_ONE_side
TITLE: Probability Properties
DESCRIPTION: - $P(\Omega) = 1$
> - $𝑃 (𝐴) = 0 ⇔ 𝐴 = ∅$ - только [[Empty Set]]  имеет нулевую вероятность
> - $P(A \sqcup B ) = P(A) + P(B)$ - $A, B$ are disjoint sets
> - $𝑃 (𝐴 ∪ 𝐵) = 𝑃(𝐴)+𝑃(𝐵)−𝑃(𝐴∩𝐵)$ - для произвольных событий
>	- [[Inclusion-Exclusion principle]]
> - $P(A,\cup...\cup A_k)\leq P(A_1)+...+P(A_k)$
> - $\bar{A}:=\Omega\backslash A\text{ paвна }P(\bar{A})=1-P(A)$
ID: 1697972721278
END
