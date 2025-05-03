---
aliases: 
tags:
  - person👤
created: 2025-04-14 20:25
connected:
  - "#обс/linking"
---
[Yao Lu](https://arxiv.org/search/cs?searchtype=author&query=Lu,+Y), [Max Bartolo](https://arxiv.org/search/cs?searchtype=author&query=Bartolo,+M), [Alastair Moore](https://arxiv.org/search/cs?searchtype=author&query=Moore,+A), [Sebastian Riedel](https://arxiv.org/search/cs?searchtype=author&query=Riedel,+S), [Pontus Stenetorp](https://arxiv.org/search/cs?searchtype=author&query=Stenetorp,+P)

https://aclanthology.org/2022.acl-long.556/
https://arxiv.org/abs/2104.08786



```
@inproceedings{lu-etal-2022-fantastically,
    title = "Fantastically Ordered Prompts and Where to Find Them: Overcoming Few-Shot Prompt Order Sensitivity",
    author = "Lu, Yao  and
      Bartolo, Max  and
      Moore, Alastair  and
      Riedel, Sebastian  and
      Stenetorp, Pontus",
    editor = "Muresan, Smaranda  and
      Nakov, Preslav  and
      Villavicencio, Aline",
    booktitle = "Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = may,
    year = "2022",
    address = "Dublin, Ireland",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.acl-long.556/",
    doi = "10.18653/v1/2022.acl-long.556",
    pages = "8086--8098",
    abstract = "When primed with only a handful of training samples, very large, pretrained language models such as GPT-3 have shown competitive results when compared to fully-supervised, fine-tuned, large, pretrained language models. We demonstrate that the order in which the samples are provided can make the difference between near state-of-the-art and random guess performance: essentially some permutations are {\textquotedblleft}fantastic{\textquotedblright} and some not. We analyse this phenomenon in detail, establishing that: it is present across model sizes (even for the largest current models), it is not related to a specific subset of samples, and that a given good permutation for one model is not transferable to another. While one could use a development set to determine which permutations are performant, this would deviate from the true few-shot setting as it requires additional annotated data. Instead, we use the generative nature of language models to construct an artificial development set and based on entropy statistics of the candidate permutations on this set, we identify performant prompts. Our method yields a 13{\%} relative improvement for GPT-family models across eleven different established text classification tasks."
}
```