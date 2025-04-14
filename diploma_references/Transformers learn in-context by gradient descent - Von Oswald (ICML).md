---
publish: true
created: 2025-04-14 20:51
doi: https://proceedings.mlr.press/v202/von-oswald23a.html
author: 
tags:
  - paper
---

https://proceedings.mlr.press/v202/von-oswald23a.html

```

@InProceedings{pmlr-v202-von-oswald23a,
  title = 	 {Transformers Learn In-Context by Gradient Descent},
  author =       {Von Oswald, Johannes and Niklasson, Eyvind and Randazzo, Ettore and Sacramento, Joao and Mordvintsev, Alexander and Zhmoginov, Andrey and Vladymyrov, Max},
  booktitle = 	 {Proceedings of the 40th International Conference on Machine Learning},
  pages = 	 {35151--35174},
  year = 	 {2023},
  editor = 	 {Krause, Andreas and Brunskill, Emma and Cho, Kyunghyun and Engelhardt, Barbara and Sabato, Sivan and Scarlett, Jonathan},
  volume = 	 {202},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {23--29 Jul},
  publisher =    {PMLR},
  pdf = 	 {https://proceedings.mlr.press/v202/von-oswald23a/von-oswald23a.pdf},
  url = 	 {https://proceedings.mlr.press/v202/von-oswald23a.html},
  abstract = 	 {At present, the mechanisms of in-context learning in Transformers are not well understood and remain mostly an intuition. In this paper, we suggest that training Transformers on auto-regressive objectives is closely related to gradient-based meta-learning formulations. We start by providing a simple weight construction that shows the equivalence of data transformations induced by 1) a single linear self-attention layer and by 2) gradient-descent (GD) on a regression loss. Motivated by that construction, we show empirically that when training self-attention-only Transformers on simple regression tasks either the models learned by GD and Transformers show great similarity or, remarkably, the weights found by optimization match the construction. Thus we show how trained Transformers become mesa-optimizers i.e. learn models by gradient descent in their forward pass. This allows us, at least in the domain of regression problems, to mechanistically understand the inner workings of in-context learning in optimized Transformers. Building on this insight, we furthermore identify how Transformers surpass the performance of plain gradient descent by learning an iterative curvature correction and learn linear models on deep data representations to solve non-linear regression tasks. Finally, we discuss intriguing parallels to a mechanism identified to be crucial for in-context learning termed induction-head (Olsson et al., 2022) and show how it could be understood as a specific case of in-context learning by gradient descent learning within Transformers.}
}

```