---
aliases:
  - Марковское свойство
anki: false
created: 2026-08-31 20:32
parent:
  - "[[Random process]]"
connected:
  - "[[Markov process]]"
tags:
  - контент/определение
---
> [!tip] Markov property
> A discrete-time stochastic process $(X_n)$ has the **Markov property** if, conditional on its present state, its next-state distribution does not depend on the earlier history:
> $$P(X_{n+1}\in A\mid X_0,\ldots,X_n)=P(X_{n+1}\in A\mid X_n)$$
> whenever these conditional probabilities are defined.

A [[Markov process]] is a random process satisfying this property.
