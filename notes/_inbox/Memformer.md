---
aliases:
  - Memory-Augmented Transformers
anki: false
created: 2024-12-19 13:20
parent:
  - "[[Transformer Architecture]]"
connected:
  - "#обс/linking"
tags:
  - empty
---


Memformers were introduced by
[Transformer-style relational reasoning with dynamic memory updating for temporal network modeling](https://ojs.aaai.org/index.php/AAAI/article/view/16583)
D Xu, J Liang, W Cheng, H Wei, H Chen, X Zhang - Proceedings of the AAAI …, 2021
Network modeling aims to learn the latent representations of nodes such that the representations preserve both network structures and node attribute information. This problem is fundamental due to its prevalence in numerous domains. However, existing approaches either target the static networks or struggle to capture the complicated temporal dependency, while most real-world networks evolve over time and the success of network modeling hinges on the understanding of how entities are temporally connected. In this paper, we present TRRN, a transformer-style relational reasoning network with dynamic memory updating, to deal with the above challenges. TRRN employs multi-head self-attention to reason over a set of memories, which provides a multitude of shortcut paths for information to flow from past observations to the current latent representations. By utilizing the policy networks augmented with differentiable binary routers, TRRN estimates the possibility of each memory being activated and dynamically updates the memories at the time steps when they are most relevant. We evaluate TRRN with the tasks of node classification and link prediction on four real temporal network datasets. Experimental results demonstrate the consistent performance gains for TRRN over the leading competitors.
