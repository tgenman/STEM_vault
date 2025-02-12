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
| Key characteristics | - Models state transitions and reward function<br><br>- Uses the model for planning and decision-making                                                                                                                                                                                                                                                                                                                                                                                                        | - Focuses on estimating value functions or directly optimizing policies<br><br>- Learns through trial and error                                                                                                                                                                                                                                                       |
| Advantages          | - Data efficiency: typically requires fewer interactions with the environment<br><br>- Better generalization to new situations                                                                                                                                                                                                                                                                                                                                                                                 | - Can work in complex environments where accurate modeling is difficult<br><br>- Often simpler to implement and computationally less demanding                                                                                                                                                                                                                        |
| Disadvantages       | - Can suffer from model errors<br>- Potentially higher computational complexity                                                                                                                                                                                                                                                                                                                                                                                                                                | - Typically requires more data/interactions with the environment<br>- May struggle with long-term planning                                                                                                                                                                                                                                                            |
| Examples            | MBPO (Model-Based Policy Optimization), Dyna-Q, World Models<br><br>- AlphaZero → Instead of playing millions of games against real opponents, it simulates its own games and learns.<br>    <br>- Self-driving cars → Testing policies in a simulator before real-world deployment.<br>    <br>- Industrial robotics → Training a robot in a virtual environment to avoid breaking expensive hardware.<br>    <br>- Drug discovery → Simulating chemical interactions instead of costly physical experiments. | Q-learning, SARSA, Policy Gradient methods (e.g., REINFORCE, PPO)<br><br>- Playing Atari games with DQN (learning purely from trial and error).<br>    <br>- Learning to walk in simulation without knowing the physics equations.<br>    <br>- Using policy gradient methods (like PPO, A3C) to train agents in complex environments (e.g., OpenAI Five for Dota 2). |
| When to use         | - In critical cases where random exploration is too risky (e.g., robotics, healthcare, self-driving cars).<br>    <br>- When you can build a simulator of the environment for safe training.<br>    <br>- When sample efficiency is important (learning faster with fewer interactions).                                                                                                                                                                                                                       | - When the environment is too complex to model accurately.<br>    <br>- When learning directly from interactions is feasible.<br>    <br>- When sample efficiency is not a major concern, and there are plenty of data or real-world interactions available.<br>    <br><br>Когда у нас есть дешевые данные✅<br><br>Пример: спотифай -> hybrid mode                   |

  
## Key Differences 🔍

### Core Trade-offs
1. **Data Efficiency** 📊
   - Model-based methods excel in sample efficiency
   - Require fewer real-world interactions
   - Learn faster from limited data

2. **Computational Aspects** 💻
   - Model-free approaches offer simpler implementation
   - Lower computational overhead
   - More straightforward training process

3. **Generalization Power** 🎯
   - Model-based methods show superior generalization
   - Better transfer to new scenarios
   - More robust understanding of environment dynamics

4. **Error Resilience** 🛡️
   - Model-free methods show higher robustness
   - No dependency on model accuracy
   - Better handling of unexpected situations

5. **Planning Capabilities** 🗺️
   - Model-based excels in strategic planning
   - Better suited for complex, long-term decisions
   - Can simulate and evaluate future scenarios

## Hybrid Approaches 🤝

Modern solutions often combine both paradigms:
- **MBVE (Model-Based Value Expansion)**
  - Enhances value estimates with model predictions
  - Balances immediate learning with planning
  
- **I2A (Imagination-Augmented Agents)**
  - Uses learned models for decision improvement
  - Combines model-free execution with model-based planning

## Recent Trends & Future Directions 🚀

1. **Rising Model-Based Interest**
   - Driven by improved data efficiency
   - Better suited for real-world applications

2. **Advanced Model Learning**
   - More sophisticated modeling techniques
   - Better uncertainty handling

3. **Deep Learning Integration**
   - Powerful function approximation
   - Enhanced representational capacity
   - State-of-the-art performance in complex domains