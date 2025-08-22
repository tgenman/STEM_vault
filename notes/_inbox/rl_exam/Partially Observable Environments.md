---
aliases: 
anki: false
created: 2025-02-12 14:14
parent:
  - "[[Environment (RL)]]"
connected:
  - "[[Fully Observable Environments]]"
  - "#обс/linking"
tags:
  - content/empty
---

- **Partial observability**: agent indirectly observes the environment:
  - A robot with camera vision isn’t told its absolute location.
  - A trading agent only observes current prices.
  - A poker playing agent only observes public cards.

- Now [[Agent State]]  $\neq$ [[Environment State]].

- Formally, this is a  [[Partially observable Markov Decision Process (PoMDP)]].

- Agent must construct its own state representation $S^a_t$, e.g.:
  - Complete history: $S^a_t = H_t$
  - Beliefs of environment state: $S^a_t = \left( \mathbb{P}[S^e_t = s^1], \dots, \mathbb{P}[S^e_t = s^n] \right)$
  - Recurrent neural network: $S^a_t = \sigma(S^a_{t-1} W_s + O_t W_o)$

