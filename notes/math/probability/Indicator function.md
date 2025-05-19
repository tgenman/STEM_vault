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
TARGET DECK: stem::math::common

START
math_complex
TITLE: Indicator function
DESCRIPTION: An ... of a subset $A$ of a set $\Omega$ is a function $I_A: \Omega \rightarrow \{0,1\}$ defined as:
FORMULA: $I_A(\omega)=\begin{cases}1,&\text{if }\omega\in A,\\0,&\text{if }\omega\notin A.\end{cases}$
ID: 1747383066471
END

START
math_basic_single
FRONT: Indicator function
$I_A(\omega)=$
BACK: $=\begin{cases}1,&\text{if }\omega\in A,\\0,&\text{if }\omega\notin A.\end{cases}$
ID: 1747383066476
END

START
math_basic_single
FRONT: Properties of Indicator function
$I_{\bar{A}} =$
BACK: $1 - I_{A}$
ID: 1747383066479
END

START
math_basic_single
FRONT: Properties of Indicator function
$\sum_{x\in \Omega}I_A(x)=$
BACK: $=|A|$
ID: 1747383066481
END

START
math_basic_single
FRONT: Properties of Indicator function
$I_{A\cap B}=$
BACK: $=I_A\cdot I_B$
ID: 1747383066483
END

START
math_basic_single
FRONT: Properties of Indicator function
$I_{A\cup B}=$
BACK: $=I_A + I_B - I_A\cdot I_B$
ID: 1747383066486
END

START
math_basic_single
FRONT: Properties of Indicator function
$I_{\emptyset}(\omega) =$
BACK: $I_{\emptyset}(\omega) = 0 \text{ for all } \omega \in \Omega$
ID: 1747383066488
END

START
math_basic_single
FRONT: Properties of Indicator function
$I_{\Omega}(\omega) =$
BACK: $= 1 \text{ for all } \omega \in \Omega$
ID: 1747383066490
END

START
math_basic_single
FRONT: Properties of Indicator function
In probability theory: $P(A) =$
BACK: $E[I_A]$
ID: 1747383066492
END
