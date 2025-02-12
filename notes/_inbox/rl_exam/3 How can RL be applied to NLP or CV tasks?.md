---
aliases: 
publish: true
anki: false
created: 2025-02-12 13:00
parent:
connected:
  - "#обс/linking"
tags:
  - empty
---


## 3.1. NLP

Motivation:

- Optimization of long-term goals (example: in dialogue systems – overall user satisfaction throughout the entire dialogue, not only the quality of individual responses),

- Working with NLP-specific quality evaluation metrics (example: non-differentiable BLEU and ROUGE that cannot be optimized by gradient descent methods),

- Learning under limited feedback conditions: IRL it can be difficult to get quick feedback on the quality of generated text. RL allows learning in such conditions using delayed and sparse reward signals.

  

Specific algorithms application:

- REINFORCE: Optimization of non-differentiable metrics in MT

- Actor-Critic: Reducing gradient variance in text generation tasks. Example: to generate image descriptions, optimizing the CIDEr metric

- DQN: Tasks with discrete action spaces, such as response selection in dialogue systems

- PPO: Stable policy training in complex language environments. OpenAI used PPO in GPT-3 for fine-tuning based on human feedback (RLHF)

- Hierarchical RL: Generation of long text sequences (example: stories)

- Inverse RL: Learning the reward function from expert demonstrations. Example: to train a summarization model based on human preferences

  

Problems:

1. High gradient variance: leads to training instability, especially in tasks with large action spaces, such as text generation

2. Difficulty in defining the reward function: can be challenging to formalize text quality as a reward

3. Slow convergence: RL usually requires more training iterations compared to supervised learning methods

4. Credit assignment problem: In long sequences, it's difficult to determine which actions led to the obtained reward

  

Promising directions:

- Combining RL with pre-trained language models (RL for fine-tuning GPT or BERT),

- Improvement of exploration methods: Developing more effective exploration strategies for learning in large action spaces characteristic of NLP tasks,

- Development of interpretable RL models: important for understanding the principles of model operation and ensuring transparency of decision-making in NLP systems.

  

## 3.2. CV

  

Motivation:

- Optimization of complex image quality metrics that can be non-differentiable (perceptual image quality (воспринимаемое правдоподобие/реализм/натуральность))

- Learning sequential processing strategies for visual information (to learn strategies for processing large images or video streams)

- Adaptation to dynamic visual environments (to adapt systems to changing visual conditions in real-time)

  

Specific algorithms application:

- Deep Q-Network (DQN): Tasks with discrete action spaces, such as object detection and image classification. Example: to learn an optimal policy for object detection by sequentially refining bounding boxes

- Policy Gradient methods (REINFORCE, A2C): Tasks with continuous action spaces, such as image transformation and enhancement. Example: to learn image cropping and enhancement policies

- DDPG (Deep Deterministic Policy Gradient): Tasks requiring continuous control, such as camera control in 3D environments. Example: to learn character animation from video demonstrations

- SAC (Soft Actor-Critic): Tasks requiring exploration and exploitation balance, such as active learning in image classification. Example: to learn an active learning policy for image classification

Task-wise:

- Image captioning: Policy Gradient, Actor-Critic. Example: REINFORCE to directly optimize CIDEr scores. Allows optimization of non-differentiable metrics and captures global sequence quality

- Active perception: DQN, A3C. Example: object recognition. Learns to focus on relevant parts of the image, reducing computational complexity and improving accuracy

- Automatic image editing: DDPG, SAC. Learns complex sequences of editing actions, adapting to image types and aesthetic preferences

- Image segmentation: DQN, Policy Gradient. Allows for adaptive refinement of segmentation with minimal user intervention

- Visual object tracking: DDPG, A3C. Adapts to changes in object appearance and background, learning long-term tracking strategies

  

Problems:

1. High computational complexity when working with high-res images

2. Difficulty in defining reward functions for visual tasks

3. Scalability issues with large and diverse datasets

4. Long training times, especially for complex tasks

  

Promising directions:

- Combining RL with self-supervised learning techniques for more efficient visual representation learning,

- Developing more sample-efficient RL algorithms for CV tasks to reduce the need for large datasets,

- Integrating RL with differentiable rendering techniques for 3D vision tasks,

- Exploring multi-agent RL for collaborative computer vision tasks, such as distributed surveillance or robot swarm coordination.

**