---
aliases:
  - Обучение с подкреплением
  - RL
created: 2025-02-11 16:09
parent:
  - "[[004.85 Machine Learning (notion)|ML]]"
connected:
  - "#обс/linking"
tags:
  - content/moc
---
![[Pasted image 20250211231823.png]]


Theoretical minima:
1. [[1 Markov decision process and its properties. Reward, discounted reward.]]
2. [[2 What is a Q-function and a Value-function? Relationship between them]]
3. [[3 How can RL be applied to NLP or CV tasks?]]
4. [[4 Exploration-exploitation tradeoff]]
5. [[5 Value-based vs. Policy based methods (general idea)]]
6. [[6 What is the difference between model-based and model-free RL?]]

Exam program:
7. Cross-entropy method (tabular and approximate case).
8. Value-based RL: state value and state-action value functions. Value-based policy iteration algorithm.
9. Value iteration algorithm.
10. Between them. Monte Carlo vs TD update questions. Q-leaning algorithm
11. Model-free RL: Bellman-expectation equality, algorithms.
12. SARSA, Expected value SARSA, Q-Learning, DQN, training details. On-policy vs. Off-policy
13. Policy-based methods. SARSA algorithm

14. Approximate Value-Based and Policy-Based Methods (without policy baselines, with policy gradient).
15. RL Advanced Policy Gradient: actor-critic algorithm.
16. RL Solvers and Deviation-Soft ActorCritic, A3C.
17. Bandit, NE Policy Gradient, REINFORCE
18. DDPG in RL algorithms.
19. Sampling. Exploration. Exploration strategies: greedy, UCB, Thompson sampling, heuristics for exploration.
20. Planning: Monte-Carlo tree search, metrics for exploration.







- [[Agent (RL)]] + [[Environment (RL)]] = [[Agent and Environment]]
- [[Observation (RL)]]
- [[Action (RL)]]
- [[Reward function]]

- [[State (RL)]]
    - [[History (RL)]]

- [[State (RL)]]
    - [[Environment State]]
    - [[Agent State]]
    - [[Markov state]]

- [[Policy (RL)]]

- Examples
    - [[Rat Example]]
    - [[Maze Example]]
    - [[Gridworld Example]]
    - [[Atari Example]]


- [[Fully Observable Environments]]
- [[Partially Observable Environments]]



---

#### Major Components of an RL Agent
- An RL agent may include one or more of these components:
    -  [[Policy (RL)]]] : agent’s behaviour function
    - [[V-function (RL)]]: how good is each state and/or action
    - [[Model (RL)]]: agent’s representation of the environment




## Categorizing RL agents 

- **Value Based**:
  - No Policy (Implicit)
  - Value Function

- **Policy Based**:
  - Policy
  - No Value Function

- **Actor Critic**:
  - Policy
  - Value Function

- **Model Free**:
  - Policy and/or Value Function
  - No Model

- **Model Based**:
  - Policy and/or Value Function
  - Model


![[Pasted image 20241024195754.png]]

---

### Learning and Planning
Two fundamental problems in sequential decision making:

- **Reinforcement Learning**:
  - The environment is initially unknown.
  - The agent interacts with the environment.
  - The agent improves its policy.

- **Planning**:
  - A model of the environment is known.
  - The agent performs computations with its model (without any external interaction).
  - The agent improves its policy.
  - a.k.a. deliberation, reasoning, introspection, pondering, thought, search.


---
### Prediction and Control
- Prediction: evaluate the future
    - Given a policy
- Control: optimise the future
    - Find the best policy

---




Популярные алгоритмы:
[Q-Learning](https://ru.wikipedia.org/wiki/Q-%D0%BE%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5), 
[SARSA](https://en.wikipedia.org/wiki/State%E2%80%93action%E2%80%93reward%E2%80%93state%E2%80%93action), 
DQN, 
[A3C](https://medium.com/emergent-future/simple-reinforcement-learning-with-tensorflow-part-8-asynchronous-actor-critic-agents-a3c-c88f72a5e9f2), 
[Генетический Алгоритм](https://ru.wikipedia.org/wiki/%D0%93%D0%B5%D0%BD%D0%B5%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D0%B9_%D0%B0%D0%BB%D0%B3%D0%BE%D1%80%D0%B8%D1%82%D0%BC)


