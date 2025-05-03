---
aliases: 
anki: false
created: 2024-10-24 19:27
parent:
  - "[[Agent (RL)]]"
  - "[[Environment (RL)]]"
connected:
  - "[[History (RL)]]"
tags:
  - empty
---

![[Pasted image 20241024184905.png|500]]

- At each step $t$ the [[Agent (RL)]] :
  - Executes [[Action (RL)]]  $A_t$
  - Receives [[Observation (RL)]] $O_t$
  - Receives scalar [[Reward function]] $R_t$
  
- The [[Environment (RL)]]: 
  - Receives  [[Action (RL)]] $A_t$
  - Emits [[Observation (RL)]] $O_{t+1}$
  - Emits scalar [[Reward function]] $R_{t+1}$

- $t$ increments at the environment step.
