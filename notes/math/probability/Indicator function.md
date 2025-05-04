---
aliases:
  - Индикаторная функция
anki: true
created: 2023-10-29 20:18
parent:
  - "[[Function (math)]]"
connected:
  - "[[519.21  Probability theory]]"
  - "[[Sample space]]"
  - "[[Event]]"
---

> [!tip] An **indicator function** of a subset $A$ of a set $\Omega$ 
> is a function $I_A: \Omega \rightarrow \{0,1\}$ defined as:
> $$I_A(\omega)=\begin{cases}1,&\text{if }\omega\in A,\\0,&\text{if }\omega\notin A.\end{cases}$$

# Interpretation

Imagine $\Omega$ as a target and $A$ as a marked area on the target. Randomly choosing a point $\omega$ from $\Omega$ is like throwing a dart at the target. If the dart hits area $A$, a bell rings (or a light turns on); otherwise, nothing happens. This can be expressed using the indicator function.

The function $I_A$ is defined on the entire sample space $\Omega$ and takes values 0 or 1 depending on whether the point belongs to subset $A$ or not. Each subset $A$ uniquely defines its indicator function $I_A$. Two functions $I_A$ and $I_B$ are identical if and only if the sets $A$ and $B$ are identical.

# Properties
- $I_{\bar{A}} = 1 - I_{A}$
- $\sum_{x\in \Omega}I_A(x)=|A|$
- $I_{A\cap B}=I_A\cdot I_B$
- $I_{A\cup B}=I_A + I_B - I_A\cdot I_B$
- $I_{\emptyset}(\omega) = 0 \text{ for all } \omega \in \Omega$
- $I_{\Omega}(\omega) = 1 \text{ for all } \omega \in \Omega$

# Applications in Probability Theory

In probability theory, indicator functions are used to:
- Represent events in a probability space
- Simplify calculations of expected values
- Define random variables for specific events
- Express probabilities as $P(A) = E[I_A]$

# Anki
> [!question]- Indicator function
TARGET DECK: stem::math::common
START
Math_TWO_side
TITLE: Indicator function
DESCRIPTION: An ... of a subset $A$ of a set $\Omega$ is a function $I_A: \Omega \rightarrow \{0,1\}$ defined as:
$I_A(\omega)=\begin{cases}1,&\text{if }\omega\in A,\\0,&\text{if }\omega\notin A.\end{cases}$
FORMULA: 
ADDITIONAL:
ID: 1746384273061
END

> [!question]- Properties of Indicator function
TARGET DECK: stem::math::common
START
Math_ONE_side
TITLE: Properties of Indicator function
DESCRIPTION: 
> - $I_{\bar{A}} = 1 - I_{A}$
> - $\sum_{x\in \Omega}I_A(x)=|A|$
> - $I_{A\cap B}=I_A\cdot I_B$
> - $I_{A\cup B}=I_A + I_B - I_A\cdot I_B$
> - $I_{\emptyset}(\omega) = 0 \text{ for all } \omega \in \Omega$
> - $I_{\Omega}(\omega) = 1 \text{ for all } \omega \in \Omega$
FORMULA: 
ADDITIONAL: In probability theory: $P(A) = E[I_A]$
ID: 1698688139477
END










