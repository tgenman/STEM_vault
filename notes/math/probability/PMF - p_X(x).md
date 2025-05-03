---
aliases:
  - PMF
  - Probability mass function
anki: false
created: 2024-03-20 18:02
parent:
  - "[[Discrete Random Variable]]"
connected:
  - "[[PDF - f_X(x)|PDF]]"
tags: 
---

> [!tip] Probability mass function (PMF) $p_X(x)$
$p_X(x) = P(X = x) = P(\{\omega \in \Omega \text{ s.t. } X(\omega) = x\})$
${X = x}$ - [[Event]]
For each possible value $x$ of $X$:
> 1. Collect all the possible outcomes that give rise to the event $\{X = x\}$.
> 2. Add their probabilities to obtain $p_X(x)$.

![[Pasted image 20240320183546.png|300]]

#### Properties:
- $p_X(x) \geq 0$
- $\sum_x p_X(x) = 1$
- $P(X \in S) = \sum_{x \in S} p_X(x).$

#### Anki
> [!question]- Probability mass function (PMF) $p_X(x)$
TARGET DECK: Math::Probability  
START
Math_ONE_side
TITLE: Probability mass function (PMF) $p_X(x)$
DESCRIPTION: 
$p_X(x) = P(X = x) = P(\{\omega \in \Omega \text{ s.t. } X(\omega) = x\})$
${X = x}$ - [[Event]]
For each possible value $x$ of $X$:
> 1. Collect all the possible outcomes that give rise to the event $\{X = x\}$.
> 2. Add their probabilities to obtain $p_X(x)$.
FORMULA: 
ADDITIONAL:
PICTURE: ![[Pasted image 20240320183546.png]]
ID: 1710950439103
END

> [!question]- Properties of Probability mass function (PMF) $p_X(x)$
TARGET DECK: Math::Probability  
START
Math_ONE_side
TITLE: Properties of Probability mass function (PMF) $p_X(x)$
DESCRIPTION: 
> - $p_X(x) \geq 0$
> - $\sum_x p_X(x) = 1$
> - $P(X \in S) = \sum_{x \in S} p_X(x).$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1710950439106
END