---
aliases: 
anki: false
created: 2025-02-12 14:16
parent:
  - "[[Reinforcement Learning]]"
connected:
  - "#обс/linking"
tags:
  - content/empty
---

- A **model** predicts what the environment will do next.
- $\mathbb{P}$ predicts the next state.
- $\mathbb{R}$ predicts the next (immediate) reward, e.g.:
  $$\mathbb{P}^a_{ss'} = \mathbb{P}[S_{t+1} = s' \mid S_t = s, A_t = a]$$
  $$\mathbb{R}^a_s = \mathbb{E}[R_{t+1} \mid S_t = s, A_t = a]$$
