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
  - контент/мос
---
![[Pasted image 20250211231823.png]]

[[RL Exam Topics|темы к экзамену по RL]]


Theoretical minima:
1. Markov decision process and its properties. Reward, discounted reward.
   ![[Pasted image 20250212124439.png]]
2. What is a Q-function and a Value-function? Relationship between them
3. How can RL be applied to NLP or CV tasks?
4. Exploration-exploitation tradeoff
5. Value-based vs. Policy based methods (general idea)
6. What is the difference between model-based and model-free RL?

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
    ![[Pasted image 20250212135721.png]]
18. DDPG in RL algorithms.
19. Sampling. Exploration. Exploration strategies: greedy, UCB, Thompson sampling, heuristics for exploration.
20. Planning: Monte-Carlo tree search, metrics for exploration.







- Agent (RL) + Environment (RL) = Agent and Environment
    - ![[Pasted image 20241024184905.png]]
- Observation (RL)
- Action (RL)
- Reward function

- State (RL)
    - History (RL)

- State (RL)
    - Environment State
        - ![[Pasted image 20241024190100.png]]
    - Agent State
        - ![[Pasted image 20241024190219.png]]
    - Markov state

- Policy (RL)

- Examples
    - Rat Example
        - ![[Pasted image 20241024193838.png]]
    - Maze Example
        - ![[Pasted image 20241024194552.png]]
        - ![[Pasted image 20241024194629.png]]
        - ![[Pasted image 20241024195511.png]]
        - ![[Pasted image 20241024195557.png]]
    - Gridworld Example
    - Atari Example
        - ![[Pasted image 20241024195943.png]]


- Fully Observable Environments
- Partially Observable Environments



---

#### Major Components of an RL Agent
- An RL agent may include one or more of these components:
    - Policy (RL): agent’s behaviour function
    - V-function (RL): how good is each state and/or action
    - Model (RL): agent’s representation of the environment




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
  - ![[Pasted image 20241024200046.png]]


---
### Prediction and Control
- Prediction: evaluate the future
    - Given a policy
    - ![[Pasted image 20241024200333.png]]
- Control: optimise the future
    - Find the best policy
    - ![[Pasted image 20241024200358.png]]

---




Популярные алгоритмы:
[Q-Learning](https://ru.wikipedia.org/wiki/Q-%D0%BE%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5), 
[SARSA](https://en.wikipedia.org/wiki/State%E2%80%93action%E2%80%93reward%E2%80%93state%E2%80%93action), 
DQN, 
[A3C](https://medium.com/emergent-future/simple-reinforcement-learning-with-tensorflow-part-8-asynchronous-actor-critic-agents-a3c-c88f72a5e9f2), 
[Генетический Алгоритм](https://ru.wikipedia.org/wiki/%D0%93%D0%B5%D0%BD%D0%B5%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D0%B9_%D0%B0%D0%BB%D0%B3%D0%BE%D1%80%D0%B8%D1%82%D0%BC)
