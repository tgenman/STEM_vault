---
aliases: 
publish: true
anki: false
created: 2024-10-24 19:00
parent: 
connected:
  - "[[Observation (RL)]]"
  - "[[Action (RL)]]"
  - "[[Reward]]"
tags:
  - empty
---

> [!tip] The **history** is 
the sequence of [[Observation (RL)|observations]] , [[Action (RL)|actions]] , and [[Reward|rewards]]:
  $H_t = O_1, R_1, A_1, \dots, A_{t-1}, O_t, R_t$

- i.e. all observable variables up to time $t$.
- i.e. the sensorimotor stream of a robot or embodied agent.

- What happens next depends on the history:
  - The [[Agent (RL)]] selects [[Action (RL)|actions]] .
  - The [[Environment (RL)]] selects [[Observation (RL)|observations]] / [[Reward|rewards]].

