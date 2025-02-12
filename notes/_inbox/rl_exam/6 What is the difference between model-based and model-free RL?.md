---
aliases: 
publish: true
anki: false
created: 2025-02-12 13:04
parent:
  - "[[Reinforcement Learning|RL]]"
connected:
  - "#обс/linking"
tags:
  - empty
---

|                     | [[Model-based RL]]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | [[Model-free RL]]                                                                                                                                                                                                                                                                                                                                                     |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                     | Builds an explicit model of the environment                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | Learns directly from experience without explicit environment modeling                                                                                                                                                                                                                                                                                                 |
| Key characteristics | - Models state transitions and reward function<br><br>  <br><br>- Uses the model for planning and decision-making                                                                                                                                                                                                                                                                                                                                                                                              | - Focuses on estimating value functions or directly optimizing policies<br><br>  <br><br>- Learns through trial and error                                                                                                                                                                                                                                             |
| Advantages          | - Data efficiency: typically requires fewer interactions with the environment<br><br>- Better generalization to new situations                                                                                                                                                                                                                                                                                                                                                                                 | - Can work in complex environments where accurate modeling is difficult<br><br>  <br><br>- Often simpler to implement and computationally less demanding                                                                                                                                                                                                              |
| Disadvantages       | - Can suffer from model errors<br><br>  <br><br>- Potentially higher computational complexity                                                                                                                                                                                                                                                                                                                                                                                                                  | - Typically requires more data/interactions with the environment<br><br>  <br><br>- May struggle with long-term planning                                                                                                                                                                                                                                              |
| Examples            | MBPO (Model-Based Policy Optimization), Dyna-Q, World Models<br><br>- AlphaZero → Instead of playing millions of games against real opponents, it simulates its own games and learns.<br>    <br>- Self-driving cars → Testing policies in a simulator before real-world deployment.<br>    <br>- Industrial robotics → Training a robot in a virtual environment to avoid breaking expensive hardware.<br>    <br>- Drug discovery → Simulating chemical interactions instead of costly physical experiments. | Q-learning, SARSA, Policy Gradient methods (e.g., REINFORCE, PPO)<br><br>- Playing Atari games with DQN (learning purely from trial and error).<br>    <br>- Learning to walk in simulation without knowing the physics equations.<br>    <br>- Using policy gradient methods (like PPO, A3C) to train agents in complex environments (e.g., OpenAI Five for Dota 2). |
| When to use         | - In critical cases where random exploration is too risky (e.g., robotics, healthcare, self-driving cars).<br>    <br>- When you can build a simulator of the environment for safe training.<br>    <br>- When sample efficiency is important (learning faster with fewer interactions).                                                                                                                                                                                                                       | - When the environment is too complex to model accurately.<br>    <br>- When learning directly from interactions is feasible.<br>    <br>- When sample efficiency is not a major concern, and there are plenty of data or real-world interactions available.<br>    <br><br>Когда у нас есть дешевые данные✅<br><br>Пример: спотифай -> hybrid mode                   |

  

Key differences:

- Data efficiency: Model-based methods generally more efficient
    
- Computational complexity: Model-free often simpler in implementation and computation
    
- Generalization: Model-based can potentially generalize better to new situations
    
- Robustness to model errors: Model-free more robust as they don't rely on an explicit model
    
- Planning capability: Model-based better suited for long-term planning
    

  

Hybrid approaches are possible combining model-based and model-free methods. Examples: MBVE (Model-Based Value Expansion), I2A (Imagination-Augmented Agents)

  

Recent trends (provided by Claude!):

- Increasing interest in model-based methods due to improved data efficiency

- Development of more sophisticated model learning techniques

- Integration of deep learning with model-based approaches

**