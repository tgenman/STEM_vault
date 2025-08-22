---
aliases:
  - Information State
anki: false
created: 2024-10-24 19:33
parent:
  - "[[State (RL)]]"
  - "[[Markov Decision process (MDP)]]"
connected:
  - "[[Markov Property]]"
tags:
  - fix/empty
---

An **information state** (a.k.a. **Markov state**) contains all useful information from the [[History (RL)]].

A state $S_t$ is **Markov** if and only if:
$$\mathbb{P}[S_{t+1} \mid S_t] = \mathbb{P}[S_{t+1} \mid S_1, \dots, S_t]$$

- "The future is independent of the past given the present":
  $$H_{1:t} \to S_t \to H_{t+1:\infty}$$
  
- Once the state is known, the history may be thrown away.
- i.e. The [[State (RL)]] is a sufficient [[Statistical functional]]  of the future.
- The [[Environment State]]  $S^e_t$ is Markov.
- The [[History (RL)]]  $H_t$ is Markov.
