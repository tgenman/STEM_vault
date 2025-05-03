---
aliases:
  - State-Action Value Function
anki: false
created: 2025-02-12 14:40
parent:
  - "[[Reinforcement Learning]]"
connected:
  - "[[Relationship Between V-function and Q-function]]"
tags:
  - empty
---

> [!tip] Q-function (State-Action Value Function)
The Q-function, denoted as $Q^\pi(s,a)$, is a fundamental concept in reinforcement learning that extends the [[V-function (RL)|value function]] by considering both the state and action. It quantifies the expected cumulative reward when:

1. Starting in state $s$
2. Taking action $a$ 
3. Following [[Policy (RL)|policy]] $\pi$ thereafter

Formally, it is defined as:

$${Q^{\pi}(s, a) = \mathbb{E}_{T \sim \pi \mid s_0 = s, a_0 = a} \left[ \sum_{t=0}^{\infty} \gamma^t r_t \right]}$$

where:
- $\gamma$ is the discount factor (same as in V-function)
- $r_t$ represents the reward at time step $t$
- $\mathbb{E}$ denotes the expected value over trajectories $T$
- The trajectory starts with state $s$ and action $a$, then follows policy $\pi$

### Key Properties
- Provides action-specific value estimates
- Enables direct comparison between different actions in a state
- Forms the basis for many important RL algorithms, especially Q-learning
- Helps in making optimal action selections without requiring a model of the environment

---

![[Relationship Between V-function and Q-function]]