---
aliases: 
publish: true
anki: false
created: 2025-02-12 14:33
parent:
connected:
  - "#обс/linking"
tags:
  - empty
---

> [!tip] Bellman Equations: The Fundamental Recursion of Value Functions
The Bellman equations are elegant recursive formulas that define how value functions relate current states to future outcomes. They come in two flavors, one for V-functions and one for Q-functions.

### 1. Bellman Equation for  [[V-function (RL)]]

$${V^{\pi}(s) = \mathbb{E}_{a \sim \pi(a \mid s)} \left[ r(s, a) + \gamma \mathbb{E}_{s'} V^{\pi}(s') \right]}$$

This beautiful equation tells us that the value of a state breaks down into:
- The expected immediate reward from following policy π
- The discounted value of where we might end up next

Think of it as a recursive definition: to know the value of where you are, you need to know the value of where you're going!

### 2. Bellman Equation for  [[Q-function (RL)]]

$${Q^{\pi}(s, a) = r(s, a) + \gamma \mathbb{E}_{s', a'} Q^{\pi}(s', a')}$$

Similarly, this equation shows that the value of a state-action pair consists of:
- The immediate reward for taking that action
- The discounted future value of subsequent state-action pairs

### The Brilliance of Bellman Equations

What makes these equations so powerful is their recursive nature. Instead of having to look infinitely into the future, they let us:
1. Focus on immediate rewards and just one step ahead
2. Build long-term value estimates through iteration
3. Connect present decisions to future outcomes
