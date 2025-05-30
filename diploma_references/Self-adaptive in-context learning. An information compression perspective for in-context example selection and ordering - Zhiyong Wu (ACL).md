---
created: 2025-04-14 20:34
doi: https://doi.org/10.18653/v1/2023.acl-long.79
author: 
tags:
  - paper
---
https://aclanthology.org/2023.acl-long.79/
Zhiyong Wu, Yaoxiang Wang, Jiacheng Ye, and Lingpeng Kong. 


```
@inproceedings{wu-etal-2023-self,
    title = "Self-Adaptive In-Context Learning: An Information Compression Perspective for In-Context Example Selection and Ordering",
    author = "Wu, Zhiyong  and
      Wang, Yaoxiang  and
      Ye, Jiacheng  and
      Kong, Lingpeng",
    editor = "Rogers, Anna  and
      Boyd-Graber, Jordan  and
      Okazaki, Naoaki",
    booktitle = "Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.acl-long.79/",
    doi = "10.18653/v1/2023.acl-long.79",
    pages = "1423--1436",
    abstract = "Despite the surprising few-shot performance of in-context learning (ICL), it is still a common practice to randomly sample examples to serve as context. This paper advocates a new principle for ICL: self-adaptive in-context learning. The self-adaption mechanism is introduced to help each sample find an in-context example organization (i.e., selection and permutation) that can derive the correct prediction, thus maximizing performance. To validate the effectiveness of self-adaptive ICL, we propose a general select-then-rank framework and instantiate it with new selection and ranking algorithms. Upon extensive evaluation on eight different NLP datasets, our self-adaptive ICL method achieves a 40{\%} relative improvement over the common practice setting. Further analysis reveals the enormous potential of self-adaptive ICL that it might be able to close the gap between ICL and finetuning given more advanced algorithms. Our code will be released to facilitate future research."
}
```