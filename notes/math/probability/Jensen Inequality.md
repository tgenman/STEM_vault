---
aliases:
  - Неравенство Йенсена
publish: true
anki: false
created: 2024-04-25 11:39
parent:
  - "[[Limit of function]]"
connected:
  - "#обс/linking"
tags:
  - empty
---

$\mathbb{E}[\phi(X)] \geq \phi(\mathbb{E}[X])$ for $\phi$ being a convex function.


### Theorem
If a function $f$ is convex, then:
$$f\left( \sum_{i=1}^{k} \alpha_i x_i \right) \leq \sum_{i=1}^{k} \alpha_i f(x_i),$$
where $\sum_{i=1}^{k} \alpha_i = 1$, and $\alpha_i \geq 0$.

### Proof by Induction

- **Base case**: $k = 2$ holds according to the definition of convexity.
  
- **Inductive hypothesis**: Assume the inequality holds for $k = m-1$:
  $$f\left( \sum_{i=1}^{m-1} \alpha_i x_i \right) \leq \sum_{i=1}^{m-1} \alpha_i f(x_i), \quad \sum_{i=1}^{m-1} \alpha_i = 1, \alpha_i \geq 0.$$

- **Inductive step**: Consider $k = m$:
  $$f\left( \sum_{i=1}^{m} \hat{\alpha}_i x_i \right) = f\left( \sum_{i=1}^{m-1} \hat{\alpha}_i x_i + \hat{\alpha}_m x_m \right).$$

  Applying the convexity of $f$:
  $$f\left( (1-\hat{\alpha}_m) \sum_{i=1}^{m-1} \frac{\hat{\alpha}_i}{1-\hat{\alpha}_m} x_i + \hat{\alpha}_m x_m \right) \leq (1-\hat{\alpha}_m) f\left( \sum_{i=1}^{m-1} \frac{\hat{\alpha}_i}{1-\hat{\alpha}_m} x_i \right) + \hat{\alpha}_m f(x_m).$$

  By the inductive hypothesis:
  $$(1-\hat{\alpha}_m) f\left( \sum_{i=1}^{m-1} \frac{\hat{\alpha}_i}{1-\hat{\alpha}_m} x_i \right) \leq (1-\hat{\alpha}_m) \sum_{i=1}^{m-1} \frac{\hat{\alpha}_i}{1-\hat{\alpha}_m} f(x_i).$$

  Therefore:
  $$f\left( \sum_{i=1}^{m} \alpha_i x_i \right) \leq \sum_{i=1}^{m} \alpha_i f(x_i).$$
