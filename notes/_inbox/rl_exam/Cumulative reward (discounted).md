---
aliases: 
publish: true
anki: false
created: 2024-10-24 19:06
parent:
  - "[[Reward function]]"
connected:
  - "#обс/linking"
tags:
  - empty
---



> [!tip] The discounted cumulative reward, also known as the return, 
represents the ==total reward== an [[Agent (RL)]] receives over time, with future rewards being progressively discounted. For a trajectory T, it is formally defined as:

$${R(T) = \sum_{t=0}^{\infty} \gamma^t r_t}$$

where:
- $r_t$ is the immediate reward received at time step $t$
- $\gamma \in [0,1]$ is the discount factor that determines the present value of future rewards:
  - $\gamma \approx 0$ prioritizes immediate rewards
  - $\gamma \approx 1$ values future rewards almost as much as immediate ones

Different approaches to calculating cumulative discounted reward (due to its non-trivial computation) give rise to various kinds of RL methods.

critical aspect of reinforcement learning:

- We need some initialization for V(s) for future states to calculate discounted cumulative reward at time t.
    

#### Properties of Discounting

1. Ensures Finite Values: Helps prevent infinite rewards from accumulating over an infinite horizon.
    
2. Encourages Short-Term Gains: A smaller γ (e.g., 0.5) leads to a focus on short-term rewards, while a larger γ (e.g., 0.99) encourages long-term planning​.
    
