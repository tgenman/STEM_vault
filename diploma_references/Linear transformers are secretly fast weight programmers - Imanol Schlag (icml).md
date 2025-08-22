---
created: 2025-04-16 13:13
doi: https://proceedings.mlr.press/v139/schlag21a.html
author: 
tags:
  - content/paper
---
Imanol Schlag, Kazuki Irie, and Jürgen Schmidhuber



```

@InProceedings{pmlr-v139-schlag21a,
  title = 	 {Linear Transformers Are Secretly Fast Weight Programmers},
  author =       {Schlag, Imanol and Irie, Kazuki and Schmidhuber, J{\"u}rgen},
  booktitle = 	 {Proceedings of the 38th International Conference on Machine Learning},
  pages = 	 {9355--9366},
  year = 	 {2021},
  editor = 	 {Meila, Marina and Zhang, Tong},
  volume = 	 {139},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {18--24 Jul},
  publisher =    {PMLR},
  pdf = 	 {http://proceedings.mlr.press/v139/schlag21a/schlag21a.pdf},
  url = 	 {https://proceedings.mlr.press/v139/schlag21a.html},
  abstract = 	 {We show the formal equivalence of linearised self-attention mechanisms and fast weight controllers from the early ’90s, where a slow neural net learns by gradient descent to program the fast weights of another net through sequences of elementary programming instructions which are additive outer products of self-invented activation patterns (today called keys and values). Such Fast Weight Programmers (FWPs) learn to manipulate the contents of a finite memory and dynamically interact with it. We infer a memory capacity limitation of recent linearised softmax attention variants, and replace the purely additive outer products by a delta rule-like programming instruction, such that the FWP can more easily learn to correct the current mapping from keys to values. The FWP also learns to compute dynamically changing learning rates. We also propose a new kernel function to linearise attention which balances simplicity and effectiveness. We conduct experiments on synthetic retrieval problems as well as standard machine translation and language modelling tasks which demonstrate the benefits of our methods.}
}

```