---
aliases: 
anki: false
created: 2025-02-12 14:30
parent:
  - "[[V-function (RL)|V-function (RL)]]"
  - "[[Q-function (RL)]]"
connected:
  - "#обс/linking"
tags:
  - fix/empty
---

> [!tip] The Relationship Between Value and Q-functions
The Value function (V-function) and Q-function are intimately connected and can be expressed in terms of each other through two fundamental relationships:

### From Q-function to V-function
$${V^{\pi}(s) = \mathbb{E}_{a \sim \pi(a \mid s)} Q^{\pi}(s, a)}$$

This elegant relationship tells us that the value of being in state $s$ is simply the expected Q-value over all possible actions we might take according to our policy $\pi$. In other words, it's like asking: "==What's the average value I can expect if I follow my policy from this state?=="

### From V-function to Q-function
$${Q^{\pi}(s, a) = r(s, a) + \gamma \mathbb{E}_{s'} V^{\pi}(s')}$$

This equation breaks down the Q-value into two intuitive components:
- $r(s,a)$: The immediate reward we get for taking action $a$ in state $s$
- $\gamma \mathbb{E}_{s'} V^{\pi}(s')$: The discounted future value we can expect from the next state
