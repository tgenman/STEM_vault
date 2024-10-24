---
aliases: Обучение с подкреплением
publish: true
created: 2023-05-03 21:35
---


- [[Agent (RL)]] + [[Environment (RL)]] = [[Agent and Environment]]
- [[Observation (RL)]]
- [[Action (RL)]]
- [[Reward]]

- [[State (RL)]]
	- [[History (RL)]]

- [[State (RL)]]
	- [[Environment State]]
	- [[Agent State]]
	- [[Markov state]]


### Rat Example
![[Pasted image 20241024193838.png]]

- What if agent state = last 3 items in sequence?
- What if agent state = counts for lights, bells and levers?
- What if agent state = complete sequence?

---

### Fully Observable Environments

![[Pasted image 20241024184905.png|500]]
**Full observability**: agent directly observes the environment state.

$$O_t = S^a_t = S^e_t$$

- Agent state = environment state = information state.
- Formally, this is a **Markov decision process** (MDP).
- (Next lecture and the majority of this course).

---


### Partially Observable Environments
- **Partial observability**: agent indirectly observes the environment:
  - A robot with camera vision isn’t told its absolute location.
  - A trading agent only observes current prices.
  - A poker playing agent only observes public cards.

- Now [[Agent State]]  $\neq$ [[Environment State]].

- Formally, this is a **partially observable Markov decision process** (POMDP).

- Agent must construct its own state representation $S^a_t$, e.g.:
  - Complete history: $S^a_t = H_t$
  - Beliefs of environment state: $S^a_t = \left( \mathbb{P}[S^e_t = s^1], \dots, \mathbb{P}[S^e_t = s^n] \right)$
  - Recurrent neural network: $S^a_t = \sigma(S^a_{t-1} W_s + O_t W_o)$




---

#### Major Components of an RL Agent
- An RL agent may include one or more of these components:
	- Policy: agent’s behaviour function
	- Value function: how good is each state and/or action
	- Model: agent’s representation of the environment


#### Policy
- A **policy** is the agent’s behaviour.
- It is a map from state to action, e.g.:
  - Deterministic policy: $a = \pi(s)$
  - Stochastic policy: $\pi(a \mid s) = \mathbb{P}[A_t = a \mid S_t = s]$

### Value function
- **Value function** is a prediction of future reward.
- Used to evaluate the goodness/badness of states.
- And therefore to select between actions, e.g.:
  $$v_\pi(s) = \mathbb{E}_\pi \left[ R_{t+1} + \gamma R_{t+2} + \gamma^2 R_{t+3} + \dots \mid S_t = s \right]$$

#### Model
- A **model** predicts what the environment will do next.
- $\mathbb{P}$ predicts the next state.
- $\mathbb{R}$ predicts the next (immediate) reward, e.g.:
  $$\mathbb{P}^a_{ss'} = \mathbb{P}[S_{t+1} = s' \mid S_t = s, A_t = a]$$
  $$\mathbb{R}^a_s = \mathbb{E}[R_{t+1} \mid S_t = s, A_t = a]$$

---

### Maze Example
![[Pasted image 20241024194552.png|300]]
- Rewards: -1 per time-step
- Actions: N, E, S, W
- States: Agent’s location

Maze Example: Policy
![[Pasted image 20241024194629.png|300]]
Arrows represent policy $π(s)$ for each state $s$



Maze Example: Value Function
![[Pasted image 20241024195511.png|300]]
Numbers represent the value $v_\pi(s)$ of each state $s$.


Maze Example: Model
![[Pasted image 20241024195557.png|300]]

---

Categorizing RL agents 

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
### Atari Example
Atari Example: Reinforcement Learning
![[Pasted image 20241024195943.png|400]]
- Rules of the game are unknown.
- Learn directly from interactive game-play.
- Pick actions on joystick, see pixels and scores.


Atari Example: Planning
![[Pasted image 20241024200046.png|400]]

---

### Exploration and Exploitation

- Reinforcement learning is like trial-and-error learning
- The agent should discover a good policy
- From its experiences of the environment
- Without losing too much reward along the way

- Exploration finds more information about the environment
- Exploitation exploits known information to maximise reward
- It is usually important to explore as well as exploit


---

### Prediction and Control
- Prediction: evaluate the future
	- Given a policy
- Control: optimise the future
	- Find the best policy

---

### Gridworld Example
Gridworld Example: Prediction
![[Pasted image 20241024200333.png]]
Gridworld Example: Control
![[Pasted image 20241024200358.png]]





Популярные алгоритмы:
[Q-Learning](https://ru.wikipedia.org/wiki/Q-%D0%BE%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5), 
[SARSA](https://en.wikipedia.org/wiki/State%E2%80%93action%E2%80%93reward%E2%80%93state%E2%80%93action), 
DQN, 
[A3C](https://medium.com/emergent-future/simple-reinforcement-learning-with-tensorflow-part-8-asynchronous-actor-critic-agents-a3c-c88f72a5e9f2), 
[Генетический Алгоритм](https://ru.wikipedia.org/wiki/%D0%93%D0%B5%D0%BD%D0%B5%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D0%B9_%D0%B0%D0%BB%D0%B3%D0%BE%D1%80%D0%B8%D1%82%D0%BC)

В обучении с подкреплением **машина не запоминает каждое движение, а пытается обобщить ситуации, чтобы выходить из них с максимальной выгодой**

Эта идея лежит в основе алгоритма [Q-learning](https://www.youtube.com/watch?v=aCEvtRtNO-M) и его производных (SARSA и DQN). Буква Q в названии означает слово Quality, то есть робот учится поступать наиболее качественно в любой ситуации, а все ситуации он запоминает как простой [марковский процесс](https://ru.wikipedia.org/wiki/%D0%9C%D0%B0%D1%80%D0%BA%D0%BE%D0%B2%D1%81%D0%BA%D0%B8%D0%B9_%D0%BF%D1%80%D0%BE%D1%86%D0%B5%D1%81%D1%81).

![[Pasted image 20230503214209.png]]
 Другие идут глубже и отдают эту работу нейросетям, пусть сами всё найдут. Так вместо Q-learning'а у нас появляется Deep Q-Network (DQN).




**Connected with:**
- subtype of [[Machine Learning MOC]]



