---
aliases:
  - MSE
  - RMSE
anki: false
created: 2024-04-11 15:43
parent:
  - "[[519.22 Statistic MOC]]"
connected:
  - "[[Standard error]]"
  - "[[Bias]]"
  - "[[Linear and Polynomial Regression]]"
  - "[[Total Sum of Squares (TSS or SST)]]"
tags:
  - fix/empty
---

> [!tip] The quality of a point estimate is sometimes assessed by the **mean squared error**, or MSE defined by
$\text{MSE} = \mathbb{E}(\hat{\theta} - \theta)^2$


#### Theorem
The MSE can be written as

$$ \text{MSE} = \text{bias}^2(\hat{\theta}_n) + \text{Var}(\hat{\theta}_n). $$

##### *Proof.* 
Let $\bar{\theta} = \mathbb{E}_\theta(\hat{\theta}_n)$. Then
$$
\begin{align*}
\mathbb{E}_\theta(\hat{\theta}_n - \theta)^2 &= \mathbb{E}_\theta(\hat{\theta}_n - \bar{\theta} + \bar{\theta} - \theta)^2 \\
&= \mathbb{E}_\theta(\hat{\theta}_n - \bar{\theta})^2 + 2(\bar{\theta} - \theta)\mathbb{E}_\theta(\hat{\theta}_n - \bar{\theta}) + \mathbb{E}_\theta(\bar{\theta} - \theta)^2 \\
&= (\bar{\theta} - \theta)^2 + \mathbb{E}_\theta(\hat{\theta}_n - \bar{\theta})^2 \\
&= \text{bias}^2(\hat{\theta}_n) + \text{Var}(\hat{\theta}_n)
\end{align*}
$$
where we have used the fact that $\mathbb{E}_\theta(\hat{\theta}_n - \bar{\theta}) = \bar{\theta} - \bar{\theta} = 0$.

---

Because the regression line minimizes squared errors, regression is also called **least squares**.

![[Pasted image 20230829204709.png]]


