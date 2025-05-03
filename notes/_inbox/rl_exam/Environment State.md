---
aliases: 
anki: false
created: 2024-10-24 18:59
parent:
  - "[[State (RL)]]"
  - "[[Environment (RL)]]"
connected: 
tags:
  - empty
---
> [!tip] The **environment state** $S^e_t$ is 
the [[Environment (RL)]] 's private representation.

- i.e. whatever data the environment uses to pick the next [[Observation (RL)]]/[[Reward function]].
- The environment state is not usually visible to the [[Agent (RL)]].
- Even if $S^e_t$ is visible, it may contain irrelevant information.



![[Pasted image 20241024190100.png|500]]

