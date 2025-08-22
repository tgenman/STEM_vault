---
aliases:
  - State value function
created: 2025-02-12 14:15
parent:
  - "[[Reinforcement Learning]]"
connected:
  - "#обс/linking"
tags:
  - content/empty
---

> [!tip] Value Function (V-function)
V-function $V^\pi(s)$ shows how good it is to be in state $s$ when following policy $\pi$.
It's the expected sum of rewards that an agent will get starting from state $s$ and following policy $\pi$:
$${V^{\pi}(s) = \mathbb{E}_{T \sim \pi \mid s_0 = s} \left[ \sum_{t=0}^{\infty} \gamma^t r_t \right]}$$
where:
- $\gamma \in [0,1]$ is the discount factor that determines how much we value future rewards compared to immediate ones
- $r_t$ is the immediate [[Reward function|reward]] received at time step $t$
- $\mathbb{E}$ denotes the expected value over all possible trajectories $T$ starting from state $s$ under policy $\pi$

The value function can also be expressed in a more intuitive form that shows the temporal structure of rewards:

$$v_\pi(s) = \mathbb{E}_\pi \left[ R_{t+1} + \gamma R_{t+2} + \gamma^2 R_{t+3} + \dots \mid S_t = s \right]$$

Key properties:
- Acts as a predictor of future rewards
- Provides a way to evaluate how "good" or "bad" different states are
- Helps in decision-making by allowing comparison between different states
- Forms the basis for many RL algorithms through policy evaluation and improvement

---

![[Relationship Between V-function and Q-function]]