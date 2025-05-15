---
aliases: 
anki: false
created: 2025-02-12 13:56
parent:
  - "[[Reinforcement Learning]]"
connected:
  - "#обс/linking"
tags:
  - empty
---
> [!tip] Policy in Reinforcement Learning
A policy π is the brain of an [[Agent (RL)|agent]] in a [[Markov Decision process (MDP)|MDP]], defining how it should act in any situation. It creates a mapping between states and actions, essentially serving as the agent's strategy or decision-making rule.
A policy π is formally defined as a function:
$\pi: S \rightarrow A$
where:
- $S$ represents the set of all possible states
- $A$ represents the set of all possible actions

### Types of Policies

#### 1. Deterministic Policy
- Provides a single, definite action for each state
- Formally written as: $a = \pi(s)$
- Example: "Always move right when in state X"

#### 2. Stochastic Policy
- Returns a probability distribution over possible actions
- Formally written as: $\pi(a|s) = \mathbb{P}[A_t = a | S_t = s]$
- Example: "70% chance to move right, 30% chance to move left when in state X"

![[Pasted image 20250212135721.png]]

### Special Case: Multi-Armed Bandits
While not typically considered MDPs due to their stateless nature, multi-armed bandits can be viewed as a simplified MDP with:
- A single state
- Multiple actions
- Immediate rewards
This makes them an excellent starting point for understanding policy optimization in simpler contexts.

### Key Points
- A policy represents the agent's behavior strategy
- It can be either deterministic or stochastic
- The goal in RL is to find an optimal policy that maximizes expected rewards
