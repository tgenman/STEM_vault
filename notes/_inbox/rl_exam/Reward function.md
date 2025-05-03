---
aliases: 
anki: false
created: 2024-10-24 19:07
parent:
  - "[[Reinforcement Learning]]"
connected:
  - "[[Cumulative reward (discounted)]]"
tags:
  - empty
---

> [!tip] reward function
The reward function $r(s,a)$ maps state-action pairs to numerical values, representing immediate feedback for the agent's decisions. It is defined as:
$r: S \times A \rightarrow \mathbb{R}$

The reward function is crucial because it:
- Defines what is "good" and "bad" for the agent
- Provides immediate feedback after each action
- Drives the agent to learn optimal behavior through reward maximization

#### Examples and Properties
1. **Grid World Example**:
   - +10 reward for reaching the goal state
   - -1 penalty for each movement action
   - 0 reward for all other state-action pairs

2. **Key Design Considerations**:
   - Must align with the true objectives of the task
   - Should be well-scaled and balanced
   - Needs to provide meaningful feedback signals

#### Common Challenges
1. **Reward Engineering**:
   - Unintended behaviors from poorly specified rewards
   - Difficulty in capturing complex objectives
   - Balance between sparse and dense rewards

2. **Best Practices**:
   - Focus on "what" to achieve, not "how" to achieve it
   - Keep the reward structure simple and interpretable
   - Ensure rewards reflect true task objectives

- Indicates how well the [[Agent (RL)]] is doing at step $t$.
- The [[Agent (RL)|agent's]]  job is to maximise [[Cumulative reward (discounted)]].
- [[Reward Hypothesis]]