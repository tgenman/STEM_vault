---
aliases:
  - Случайная величина
anki: true
created: 2024-03-20 11:32
parent:
  - "[[519.21  Probability theory]]"
  - "[[519.22 Statistic MOC]]"
  - "[[Randomness]]"
connected:
  - "[[Discrete Random Variable]]"
  - "[[General Random Variables]]"
  - "[[Moment of r.v.]]"
tags:
---

> [!tip] Random Variable (r.v.) X (def 1)
A random variable is a real-valued function of the outcome of the  [[Random experiment|experiment]]
A function from the sample space $\Omega$ to the real numbers


> [!tip] Random Variable (r.v.) X (def 2)
действительная функция от [[Elementary event|элементарнорго исхода]]$\xi=\xi(\omega),\omega\in \Omega$, для которой при любом действительном $x$ множество $\{\omega:\xi(\omega)\le x\}$ принадлежит $\mathcal{A}$, то есть является событием, и для него определена вероятность $P\{\omega:\xi(\omega)\le x\}$.

Пусть дано $\Omega$ и заданы вероятности $P$ каждого из элементарных исходов в этом пространстве. 
Назовем случайной величиной **любую** функцию $\xi: \Omega \rightarrow \mathbb{R}$.


#### Properties
- A  [[Function (math)|function]] of a ==random variable== defines another ==random variable==. - [[Functions of random variables]]
- We can associate with each random variable certain "averages" of interest, such as the [[Expected Value E(X)]]  and [[Variance V(X)]] .
- A ==random variable== can be [[Conditional Probability|conditioned]]  on an [[Event]] or on another ==random variable==.
- There is a notion of [[Independence]] of a ==random variable== from an [[Event]] or from another ==random variable==.

#### Пример

Пусть $\Omega$ — это пространство исходов броска игральной кости $\Omega=\{1,2,3,4,5,6\}$
Возьмем любую функцию, например $\xi(\omega) = \omega^2$ или $\xi(\omega)=\sin \omega$


#### Anki
> [!question]- Random Variable (r.v.) X (def 1)
TARGET DECK: math::probability
START
Math_ONE_side
TITLE: Random Variable (r.v.) X (def 1)
DESCRIPTION: A random variable is a real-valued function of the outcome of the  [[Random experiment|experiment]]
A function from the sample space $\Omega$ to the real numbers
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1710946167831
END

> [!question]- Random Variable (r.v.) X (def 2)
TARGET DECK: math::probability
START
Math_ONE_side
TITLE: Random Variable (r.v.) X (def 2)
DESCRIPTION: 
действительная функция от [[Elementary event|элементарнорго исхода]]$\xi=\xi(\omega),\omega\in \Omega$, для которой при любом действительном $x$ множество $\{\omega:\xi(\omega)\le x\}$ принадлежит $\mathcal{A}$, то есть является событием, и для него определена вероятность $P\{\omega:\xi(\omega)\le x\}$.
FORMULA: 
Пусть $\Omega$ — это пространство исходов броска игральной кости $\Omega=\{1,2,3,4,5,6\}$
Возьмем любую функцию, например $\xi(\omega) = \omega^2$ или $\xi(\omega)=\sin \omega$
ADDITIONAL:
Пусть дано $\Omega$ и заданы вероятности $P$ каждого из элементарных исходов в этом пространстве. 
Назовем случайной величиной **любую** функцию $\xi: \Omega \rightarrow \mathbb{R}$.
PICTURE:
ID: 1710946741413
END

> [!question]- Properties of Random Variable (r.v.) X
TARGET DECK: math::probability
START
Math_ONE_side
TITLE: Properties of Random Variable (r.v.) X
DESCRIPTION: 
> - A  [[Function (math)|function]] of a ==random variable== defines another ==random variable==.
> - We can associate with each random variable certain "averages" of interest, such as the [[Expected Value E(X)]]  and [[Variance V(X)]] .
> - A ==random variable== can be [[Conditional Probability|conditioned]]  on an [[Event]] or on another ==random variable==.
> - There is a notion of [[Independence]] of a ==random variable== from an [[Event]] or from another ==random variable==.
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1710946167836
END