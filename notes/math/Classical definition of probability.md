---
aliases:
  - Классическое определение вероятности
anki: true
created: 2023-10-20 20:39
parent:
  - "[[Probability]]"
connected:
---
##### Classical definition of probability 
$\Omega = \{\omega_1, ..., \omega_n\}$ - [[Sample space]] of [[Elementary event]]s
$A \subset \Omega$ - [[Event]]
$P(A) = \frac{|A|}{n}$ - [[Probability]] [[Probability measure]]

##### Probability Axioms
- Nonnegativity $P(A) >= 0$
- Normalization $P(\Omega) = 1$
- Additivity $P(A \sqcup B ) = P(A) + P(B)$ -  where $A, B$ are disjoint sets

##### Discrete Probability Law
> [!tip] Discrete Probability Law
If the sample space consists of a finite number of possible outcomes, then the probability law is specified by the probabilities of the events that consist of a single element. In particular, the probability of any event $\{s_1, s_2, \ldots, s_n\}$ is the sum of the probabilities of its elements:
$P(\{s_1, s_2, \ldots, s_n\}) = P(s_1) + P(s_2) + \ldots + P(s_n)$

##### Discrete Uniform Probability Law
> [!tip] Discrete Uniform Probability Law
If the sample space consists of $n$ possible outcomes which are equally likely (i.e., all single-element events have the same probability), then the probability of any event $A$ is given by
$P(A) = \frac{\text{number of elements of } A}{n}$

##### Some Properties of Probability Laws
- $𝑃 (𝐴) = 0 ⇔ 𝐴 = ∅$ - только [[Empty Set]]  имеет нулевую вероятность
- If $A \subset B$, then $P(A) \leq P(B)$.
- $𝑃 (𝐴 ∪ 𝐵) = 𝑃(𝐴)+𝑃(𝐵)−𝑃(𝐴∩𝐵)$ -  [[Sum Rule of Probability]]
- $P(A,\cup...\cup A_k)\leq P(A_1)+...+P(A_k)$
	- $P(A \cup B) \leq P(A) + P(B)$.
- $\bar{A}:=\Omega\backslash A$  =>  $P(\bar{A})=1-P(A)$
- $P(A \cup B \cup C) = P(A) + P(A^c \cap B) + P(A^c \cap B^c \cap C)$.



### Anki
> [!question]- Classical definition of probability
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Classical definition of probability
DESCRIPTION: 
> $\Omega = \{\omega_1, ..., \omega_n\}$ - [[Sample space]] of [[Elementary event]]s
> $A \subset \Omega$ - [[Event]]
> $P(A) = \frac{|A|}{n}$ - [[Probability]]
ID: 1697972721265
END

> [!question]- Probability Axioms
START
Math_ONE_side
TITLE: Probability Axioms
DESCRIPTION: 
> - Nonnegativity $P(A) >= 0$
> - Normalization $P(\Omega) = 1$
> - Additivity $P(A \sqcup B ) = P(A) + P(B)$ -  where $A, B$ are disjoint sets
ID: 1697972721278
END

> [!question]- Discrete Probability Law
START
Math_TWO_side
TITLE: Discrete Probability Law
DESCRIPTION: If the sample space consists of a finite number of possible outcomes, then the probability law is specified by the probabilities of the events that consist of a single element. In particular, the probability of any event $\{s_1, s_2, \ldots, s_n\}$ is the sum of the probabilities of its elements:
> $P(\{s_1, s_2, \ldots, s_n\}) = P(s_1) + P(s_2) + \ldots + P(s_n)$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1709888037333
END

> [!question]- Discrete Uniform Probability Law
START
Math_TWO_side
TITLE: Discrete Uniform Probability Law
DESCRIPTION: If the sample space consists of $n$ possible outcomes which are equally likely (i.e., all single-element events have the same probability), then the probability of any event $A$ is given by
> $P(A) = \frac{\text{number of elements of } A}{n}$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1709888037335
END

> [!question]- Some Properties of Probability Laws
START
Math_ONE_side
TITLE: Some Properties of Probability Laws
DESCRIPTION: 
> - $𝑃 (𝐴) = 0 ⇔ 𝐴 = ∅$ - только [[Empty Set]]  имеет нулевую вероятность
> - If $A \subset B$, then $P(A) \leq P(B)$.
> - $𝑃 (𝐴 ∪ 𝐵) = 𝑃(𝐴)+𝑃(𝐵)−𝑃(𝐴∩𝐵)$ -  [[Inclusion-Exclusion principle]]
> - $P(A,\cup...\cup A_k)\leq P(A_1)+...+P(A_k)$
> 	- $P(A \cup B) \leq P(A) + P(B)$.
> - $\bar{A}:=\Omega\backslash A$  =>  $P(\bar{A})=1-P(A)$
> - $P(A \cup B \cup C) = P(A) + P(A^c \cap B) + P(A^c \cap B^c \cap C)$.
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1709888037336
END