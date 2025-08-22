---
aliases: 
anki: false
created: 2025-02-12 13:08
parent:
  - "[[Markov Decision process (MDP)]]"
connected:
  - "#обс/linking"
tags:
  - content/empty
---

> [!tip] The transition function $P(s'|s,a)$ 
represents the dynamics of the environment by specifying the probability of transitioning to a new [[State (RL)]]  given the current state and [[Action (RL)]]:
- **Definition**: A probability distribution that determines the likelihood of reaching state $s'$ when taking action $a$ in state $s$
- **Purpose**: Models the environment's response to agent actions
- **Properties**: For any state $s$ and action $a$, the sum of probabilities over all possible next states equals 1

#### Examples and Properties

1. **Deterministic Environment Example**:
   - Moving right in a grid world always leads to the right cell
   - $P(s'|s,a) = 1$ for the intended next state
   - $P(s'|s,a) = 0$ for all other states

2. **Stochastic Environment Example**:
   - Robot movement with uncertainty
   - 80% chance of moving as intended
   - 10% chance of moving left/right of intended direction

#### Key Characteristics
1.  [[Markov Property]]:
   - Next state depends only on current state and action
   - Past history is irrelevant given current state
   - Enables efficient planning and learning

2. **Practical Considerations**:
   - May be unknown in real-world applications
   - Can be learned through experience
   - Often approximated in complex environments

