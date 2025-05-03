---
created: 2025-04-14 20:49
doi: https://doi.org/10.18653/v1/2023.findings-acl.247
author: 
tags:
  - paper
---

Damai Dai, Yutao Sun, Li Dong, Yaru Hao, Shuming Ma, Zhifang Sui, and Furu Wei. 2023

```
@inproceedings{dai-etal-2023-gpt,
    title = "Why Can {GPT} Learn In-Context? Language Models Secretly Perform Gradient Descent as Meta-Optimizers",
    author = "Dai, Damai  and
      Sun, Yutao  and
      Dong, Li  and
      Hao, Yaru  and
      Ma, Shuming  and
      Sui, Zhifang  and
      Wei, Furu",
    editor = "Rogers, Anna  and
      Boyd-Graber, Jordan  and
      Okazaki, Naoaki",
    booktitle = "Findings of the Association for Computational Linguistics: ACL 2023",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.findings-acl.247/",
    doi = "10.18653/v1/2023.findings-acl.247",
    pages = "4005--4019",
    abstract = "Large pretrained language models have shown surprising in-context learning (ICL) ability. With a few demonstration input-label pairs, they can predict the label for an unseen input without parameter updates. Despite the great success in performance, its working mechanism still remains an open question. In this paper, we explain language models as meta-optimizers and understand in-context learning as implicit finetuning. Theoretically, we figure out that Transformer attention has a dual form of gradient descent. On top of it, we understand ICL as follows: GPT first produces meta-gradients according to the demonstration examples, and then these meta-gradients are applied to the original GPT to build an ICL model. We comprehensively compare the behaviors of in-context learning and explicit finetuning on real tasks to provide empirical evidence that supports our understanding. Experimental results show that in-context learning behaves similarly to explicit finetuning from multiple perspectives. Inspired by the dual form between Transformer attention and gradient descent, we design a momentum-based attention by analogy with gradient descent with momentum. The improved performance over vanilla attention further supports our understanding from another perspective, and more importantly, shows the potential to utilize our understanding for future model design. The code is available at \url{https://aka.ms/icl}."
}
```