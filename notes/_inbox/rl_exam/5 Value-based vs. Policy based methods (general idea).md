---
aliases: 
publish: true
anki: false
created: 2025-02-12 13:03
parent:
connected:
  - "#обс/linking"
tags:
  - empty
---
**

### 1. Value-based Methods

- These methods focus on learning a value function V, which estimates how good it is for the agent to be in a given state or take a specific action.
    
- The agent indirectly derives a policy from the learned value function by choosing the action that maximizes the expected future reward.
    
- A well-known example of value-based RL is Deep Q-Networks (DQN), which learns the Q-function using experience replay and deep neural networks​.
    
- Key properties:
    

- Works in an off-policy manner, meaning it can learn from stored experiences rather than requiring fresh data every time.
    
- Sample-efficient compared to policy-based methods.
    
- Prone to instability and divergence due to approximating a complex Q-function.
    

### 2. Policy-based Methods

- These methods learn a policy directly, meaning they parameterize and optimize the policy function without relying on a value function.
    
- The policy function determines the probability of selecting each action given a state.
    
- Policy Gradient Methods (such as REINFORCE and Proximal Policy Optimization, PPO) adjust the parameters of the policy using gradient ascent on expected rewards​.
    
- Key properties:
    

- Works in an on-policy manner, meaning it requires fresh interactions with the environment.
    
- More effective for continuous action spaces where value-based methods struggle.
    
- Higher variance but can converge to better solutions for complex tasks.
    

### Comparison

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeKRN7li2Y8ox-M5Ka1GCwlj-HwU0ZwJN0EiACvg7J6XospaEh5OmyurG0hH0OmZVH8jfbWRpXFTtx0sHSH4WjOaNskgs8rfo8Zw0dgNM9642Kl72nvnsk3q5O_5xeXIqwSE32THw?key=bLVzrIeeji0xOX_OWgzfwxJh)

### Summary

- Value-based methods like DQN learn a Q-function and derive the policy from it. They are sample-efficient but struggle in high-dimensional continuous action spaces.
    

- Value-based methods like DQN struggle in high-dimensional continuous action spaces because they require evaluating the Q-value for every possible action, which is infeasible when actions are continuous. Instead, policy-based methods (like actor-critic) are preferred since they can directly learn a parameterized policy to select actions without needing to discretize or exhaustively search the action space.
    

- Policy-based methods directly optimize the policy and perform better in complex environments, but they suffer from higher variance and require fresh data constantly.
    
- Many modern RL algorithms, such as Actor-Critic methods, combine both approaches to leverage their strengths​.
    

Можно добавить конкретные примеры когда какую выбрать и конкретные юзкейсы

### When to Choose Value-Based Methods (e.g., DQN, Double DQN, Dueling DQN)

✅ Best for: Discrete action spaces with a manageable number of actions

1. Atari Games (DQN) – The action space consists of a few discrete moves (e.g., left, right, jump), making Q-learning feasible.
    
2. Chess, Go (AlphaZero-like approaches) – A finite set of valid moves at each state allows Q-function learning.
    
3. Inventory Management – Discrete decisions like "order stock or not" are well-suited for Q-learning.
    
4. Gridworld Navigation – The agent chooses among discrete moves like up, down, left, or right.
    
5. Turn-based Strategy Games – Limited action choices make value-based methods practical.
    

### When to Choose Policy-Based Methods (e.g., REINFORCE, PPO, A3C, SAC)

✅ Best for: Continuous or complex action spaces, or when learning a stochastic policy is beneficial

6. Robotics Control (PPO, SAC, DDPG) – Actions (e.g., joint torques, velocities) are continuous, making Q-learning impractical.
    
7. Autonomous Driving (TD3, SAC) – Continuous steering, acceleration, and braking require a policy-based approach.
    
8. Finance & Trading (PPO, A2C) – Continuous decisions like adjusting investment ratios benefit from policy learning.
    
9. Playing Soccer in Simulation (PPO, A3C) – Agents need to move in all directions smoothly rather than pick discrete moves.
    
10. Game AI for FPS games (PPO, SAC) – Aiming, movement, and reaction timing require continuous control.
    

**