---
aliases: 
publish: true
anki: false
created: 2025-02-09 22:49
parent: 
connected:
  - "#обс/linking"
tags:
  - empty
  - группа
---


**

### 1. Transformer Architecture: Block Structure

The Transformer architecture consists of encoder and decoder stacks, each composed of identical layers. Below is the structure of each component.

#### 1.1 Encoder Block

- The encoder block processes input sequences and outputs contextualized representations.
    

##### Components:

1. Multi-Head Self-Attention:
    

- Each token attends to every other token in the sequence, capturing global dependencies.
    
- Consists of multiple attention "heads" running in parallel.
    

2. Feedforward Network (FFN):
    

- Two fully connected layers with a non-linear activation function (e.g., ReLU) in between.
    
- Applies independently to each token position.
    

3. Residual Connections:
    

- Adds the input of each sublayer (e.g., attention or FFN) to its output to facilitate gradient flow.
    

4. Layer Normalization:
    

- Applied after the residual connection to stabilize and normalize the layer outputs.
    

##### Structure of an Encoder Block:

Output=LayerNorm(Residual+SubLayerOutput)

#### 1.2 Decoder Block

- The decoder block generates sequences conditioned on encoder outputs.
    

##### Additional Component:

5. Masked Multi-Head Self-Attention:
    

- Ensures that each position in the sequence can only attend to earlier positions (causal masking).
    
- Used for auto-regressive generation.
    

6. Encoder-Decoder Attention:
    

- Enables the decoder to attend to encoder outputs, incorporating information from the input sequence.
    

##### Structure of a Decoder Block:

7. Masked Multi-Head Attention → Add & Norm
    
8. Encoder-Decoder Attention → Add & Norm
    
9. Feedforward Network → Add & Norm
    

### 2. Layer Normalization (Layer Norm)

Layer normalization plays a critical role in stabilizing training. It normalizes the inputs across the features for each token independently.

#### Equation:
Layer normalization is computed as:  
$${\text{LayerNorm}(x) = \frac{x - \mu}{\sqrt{\sigma^2 + \epsilon}} \cdot \gamma + \beta}$$  

- ${x}$: Input vector.  
- ${\mu, \sigma^2}$: Mean and variance of the input vector.  
- ${\gamma, \beta}$: Learnable parameters for scaling and shifting.  
- ${\epsilon}$: Small constant to avoid division by zero.  

Layer norm is applied after the residual connections in each sublayer.

### 3. Training Procedure

#### 3.1 Optimizer: AdamW

AdamW (Adam with weight decay) is a popular optimizer for training Transformers. It is an improved version of the Adam optimizer.

##### Key Features:

- Weight Decay:
    

- Decouples the weight decay (L2 regularization) from gradient updates.
    
- Improves generalization and avoids over-regularizing moving averages in Adam.
    

- Gradient Update Rule:
    The update rules for the optimizer are:  

$${m_t = \beta_1 m_{t-1} + (1 - \beta_1) \nabla L(\theta_t)}$$  
$${v_t = \beta_2 v_{t-1} + (1 - \beta_2)(\nabla L(\theta_t))^2}$$  
$${\hat{\theta}_{t+1} = \theta_t - \eta \cdot \frac{m_t}{\sqrt{v_t + \epsilon}} - \eta \cdot \lambda \cdot \theta_t}$$  

- ${m_t}$: Exponentially weighted moving average of the gradients.  
- ${v_t}$: Exponentially weighted moving average of the squared gradients.  
- ${\eta}$: Learning rate.  
- ${\beta_1, \beta_2}$: Decay rates for the moving averages.  
- ${\epsilon}$: Small constant to improve numerical stability.  
- ${\lambda}$: Weight decay coefficient.  

#### 3.2 Learning Rate Scheduling

Training Transformers involves using learning rate (LR) scheduling to balance stability and speed during optimization.

##### Warmup + Decay:

- Warmup Phase:
    

- Gradually increase the learning rate from a small value over a specified number of steps.
    

- Decay Phase:
    

- After warmup, the learning rate decays according to a schedule (e.g., inverse square root, cosine decay).
    

##### Common Schedule:
The learning rate schedule is defined as:  
$${\eta_t = \eta_{\text{max}} \cdot \min\left(t^{-0.5}, t \cdot \text{warmup\_steps}^{-1.5}\right)}$$  

- ${\eta_{\text{max}}}$: Maximum learning rate.  
- ${t}$: Current training step.  
- ${\text{warmup\_steps}}$: Number of warmup steps.  

#### 3.3 Label Smoothing

Label smoothing mitigates overconfidence in predictions by assigning small probabilities to incorrect classes in the target distribution.

##### Smoothed Target Distribution:

The smoothed probability ${q(k)}$ is defined as:  
$${q(k) = \begin{cases} 
1 - \epsilon & \text{if } k = y \ (\text{true label}) \\ 
\frac{\epsilon}{K-1} & \text{if } k \neq y 
\end{cases}}$$  

- ${q(k)}$: Smoothed probability for class ${k}$.  
- ${y}$: True class.  
- ${\epsilon}$: Smoothing factor (e.g., ${\epsilon = 0.1}$).  
- ${K}$: Number of classes.  

    

##### Advantages:

- Reduces overfitting by discouraging the model from assigning 100% probability to the correct class.
    
- Improves calibration and generalization.
    

**