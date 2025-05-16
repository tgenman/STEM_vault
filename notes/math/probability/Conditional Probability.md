---
aliases:
  - Условная вероятность
anki: true
created: 2023-07-07 10:02
parent:
  - "[[Probability]]"
  - "[[519.21  Probability theory]]"
connected:
  - "[[The multiplication rule (conditional probability)]]"
  - "[[Total Probability Theorem]]"
  - "[[Bayes' Rule|Bayes’ Theorem]]"
tags: 
---

> [!tip] The conditional probability $\mathbb{P}(A|B)$
 is the probability of event $A$ calculated with just the outcomes where the condition $B$ holds.
 $P(A | B) = \frac{P(A \cap B)}{P(B)} = \frac{|A \cap B|}{|B|}$ 

Нaзывают еще теоремой умножения:
$$P(A|B)P(B) = P(A \cap B)$$
![[Pasted image 20240320164442.png|300]]
#### Properties
- Conditional probabilities can also be viewed as a probability law on a new universe $B$, because all of the conditional probability is concentrated on $B$.
- If the possible outcomes are  [[Classical definition of probability|finitely many]] and equally likely, then
$P(A | B) = \frac{\text{number of elements of } A \cap B}{\text{number of elements of } B}.$
- [[The multiplication rule (conditional probability)]]


###### Example
Event $A$: Airplane is flying above
Event $B$: Something registers on radar screen
![[Pasted image 20240320165213.png|300]]

- $P(A \cap B) = P(A) \cdot P(B | A) = 0.05 \cdot 0.99$
- $P(B) = 0.05 \cdot 0.99 + 0.95 \cdot 0.1 = 0.1445$
- $P(A | B) = \frac{0.05 \cdot 0.99}{0.1445} = 0.34$

$P(A | B) = \frac{P(A \cap B)}{P(B)}$



# Anki
TARGET DECK: math::probability
START
math_complex
TITLE: The conditional probability $\mathbb{P}(A|B)$
DESCRIPTION: is the probability of event $A$ calculated with just the outcomes where the condition $B$ holds.
FORMULA:  $P(A | B) = \frac{P(A \cap B)}{P(B)} = \frac{|A \cap B|}{|B|}$
$$P(A|B)P(B) = P(A \cap B)$$
$P(A | B) = \frac{\text{number of elements of } A \cap B}{\text{number of elements of } B}.$
ADDITIONAL: 
- Conditional probabilities can also be viewed as a probability law on a new universe $B$, because all of the conditional probability is concentrated on $B$.
- If the possible outcomes are  [[Classical definition of probability|finitely many]] and equally likely, then
> $P(A | B) = \frac{\text{number of elements of } A \cap B}{\text{number of elements of } B}.$
> [[The multiplication rule (conditional probability)]]
> ![[Pasted image 20240320164442.png]]
ID: 1702137389003
END

TARGET DECK: math::probability
START
math_complex
TITLE: Example of conditional probability
DESCRIPTION:
> Event $A$: Airplane is flying above
> Event $B$: Something registers on radar screen
> ![[Pasted image 20240320165213.png|300]]
- $P(A \cap B) = P(A) \cdot P(B | A) = 0.05 \cdot 0.99$
- $P(B) = 0.05 \cdot 0.99 + 0.95 \cdot 0.1 = 0.1445$
- $P(A | B) = \frac{0.05 \cdot 0.99}{0.1445} = 0.34$
> $P(A | B) = \frac{P(A \cap B)}{P(B)}$
FORMULA:  
ADDITIONAL: 
ID: 1710942863144
END