---
aliases: 
anki: false
created: 2025-02-12 12:41
parent:
  - "[[Reinforcement Learning|RL]]"
connected:
  - "#обс/linking"
tags:
  - fix/empty
  - fix/study_group
---
- [[Markov Decision process (MDP)]]
- [[Transition function]]
- [[Reward function]]
- [[Cumulative reward (discounted)]]
- [[Policy (RL)]]

**

A ==Markov Decision Process (MDP)== is a mathematical framework that forms the foundation of reinforcement learning. It elegantly models sequential decision-making scenarios where:
- The outcomes are partially stochastic (random)
- And partially controlled by an agent's actions

Formally, an MDP is defined as a tuple $(S, A, P, r)$ consisting of:
- **[[State (RL)]] Space**  $S$: The set of all possible situations or configurations that the environment can be in
- **[[Action (RL)]] Space** $A$: The complete set of actions that the agent can choose from
- **[[Transition function]]** $P(s'|s,a)$: A probability distribution that determines how likely it is to reach state $s'$ when taking action $a$ in state $s$
- **[[Reward function]]** $r(s,a)$: A mapping that specifies the immediate reward the agent receives for taking action $a$ while in state $s$

This structure captures the [[Markov Property]], which states that the future state depends only on the present state and action, not on past states or actions​.
![[Pasted image 20250212124439.png]]



