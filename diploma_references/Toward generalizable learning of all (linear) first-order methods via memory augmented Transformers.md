---
publish: true
created: 2025-04-14 19:02
doi: https://doi.org/10.48550/arXiv.2410.07263
tags:
  - paper
author:
  - "[[Sanchayan Dutta]]"
  - "[[Suvrit Sra]]"
---

## Thinking
Давайте разберем, как матрица X связана с матрицей Z₀.

Z₀ - это расширенная версия матрицы X, которая включает в себя как признаки, так и отклики. Она имеет специальную структуру из двух строк блоков:

```
Z₀ = [x(1)   x(2)   ...   x(n)   x(n+1)]  # Верхний блок - признаки
     [y(1)   y(2)   ...   y(n)     0   ]  # Нижний блок - отклики
```

Размерность Z₀ равна (d+1)×(n+1), где:
- d+1 строк (d строк для признаков + 1 строка для откликов)
- n+1 столбцов (n примеров + 1 точка для предсказания)

Связь между X и Z₀ следующая:
1. Верхний блок Z₀ содержит транспонированную матрицу X. То есть если в X признаки были строками, то в Z₀ они становятся столбцами.
2. Нижняя строка Z₀ содержит соответствующие отклики y(i) = ⟨x(i),w*⟩ для каждого примера, а для последней точки x(n+1) стоит 0, так как это значение нужно предсказать.

Например, если у нас d=2 (два признака) и n=3 (три обучающих примера), то:

Матрица X будет размера 4×2:
```
X = [1.0  2.0]  # x(1)
    [3.0  4.0]  # x(2)
    [5.0  6.0]  # x(3)
    [7.0  8.0]  # x(n+1)
```

А соответствующая матрица Z₀ будет размера 3×4:
```
Z₀ = [1.0  3.0  5.0  7.0]  # Первый признак
     [2.0  4.0  6.0  8.0]  # Второй признак
     [y₁   y₂   y₃    0 ]  # Отклики
```

Такая структура Z₀ позволяет трансформеру одновременно видеть как признаки, так и отклики, что важно для задачи обучения в контексте.

---

Память передается между слоями внутри одного forward pass, что позволяет реализовать сложные методы оптимизации.

Убрана сеть FFN для упрощения вычислений
- ==Может просто добавить FFN и попробовать методы второго порядка?

Авторы показывают, что их архитектура может эффективно справляться с ill-conditioned problems, имитируя поведение CGD. Это важно, потому что многие задачи в машинном обучении являются плохо обусловленными, особенно при обучении глубоких нейронных сетей.


```bibtex
@misc{dutta2025generalizablelearninglinearfirstorder,
      title={Toward generalizable learning of all (linear) first-order methods via memory augmented Transformers}, 
      author={Sanchayan Dutta and Suvrit Sra},
      year={2025},
      eprint={2410.07263},
      archivePrefix={arXiv},
      primaryClass={cs.LG},
      url={https://arxiv.org/abs/2410.07263}, 
}
```

---

## References

ACL (Association for Computational Linguistics)
EMNLP (Conference on Empirical Methods in Natural Language Processing)
NAACL (North American Chapter of the Association for Computational Linguistics)
EACL (European Chapter of the Association for Computational Linguistics)
ICLR (International Conference on Learning Representations)
NeurIPS (Conference on Neural Information Processing Systems)

- [[Language models are few-shot learners - Tom B Brown (neurips)]]
- [[What makes good in-context examples for gpt-3 - Jiachang Liu (arXiv)]]
- [[Fantastically ordered prompts and where to find them. Overcoming few-shot prompt order sensitivity. - Yao Lu (ACL)]]
- [[Chain-of-thought prompting elicits reasoning in large language models. Advances in neural information processing systems - Jason Wei (neurips)]]
- [[Self-adaptive in-context learning. An information compression perspective for in-context example selection and ordering - Zhiyong Wu (ACL)]]
- [[GPT-4 Technical Report - OpenAI (arXiv)]]
- [[Llama. Open and efficient foundation language models - Hugo Touvron]]
- [[Why can gpt learn in-context? language models implicitly perform gradient descent as meta-optimizers - Damai Dai (ACL)]]
- [[Transformers learn in-context by gradient descent - Von Oswald (ICML)]]
- [[What can transformers learn in-context? a case study of simple function classes - Shivam Garg (neurips)]].
- [[What learning algorithm is in-context learning? investigations with linear models - Ekin Akyürek (arxiv)]]
- [[One step of gradient descent is provably the optimal in-context learner with one layer of linear self-attention - Arvind Mahankali (arxiv)]]
- [[Transformers learn to implement preconditioned gradient descent for in-context learning - Kwangjun Ahn (neurips)]]
- [[Transformers learn higher-order optimization methods for in-context learning. A study with linear models - Deqing Fu (arxiv)]]
- Max Vladymyrov, Johannes Von Oswald, Mark Sandler, and Rong Ge. Linear transformers are versatile in-context learners. arXiv preprint arXiv:2402.14180, 2024. 
- Gabriel Goh. Why momentum really works. Distill, 2017. doi: 10.23915/distill.00006. URL http://distill.pub/2017/momentum.
- [[Memformer. A memory-augmented transformer for sequence modeling - Qingyang Wu (ACL)]]
- Dongkuan Xu, Junjie Liang, Wei Cheng, Hua Wei, Haifeng Chen, and Xiang Zhang. Transformerstyle relational reasoning with dynamic memory updating for temporal network modeling. In Proceedings of the AAAI conference on artificial intelligence, volume 35, pages 4546–4554, 2021.
- Ruiqi Zhang, Spencer Frei, and Peter L Bartlett. Trained transformers learn linear models incontext. Journal of Machine Learning Research, 25(49):1–55, 2024.
- Imanol Schlag, Kazuki Irie, and Jürgen Schmidhuber. Linear transformers are secretly fast weight programmers. In International Conference on Machine Learning, pages 9355–9366. PMLR, 2021.
- Charlie Snell, Jaehoon Lee, Kelvin Xu, and Aviral Kumar. Scaling llm test-time compute optimally can be more effective than scaling model parameters. ICLR 2025 arXiv:2408.03314, 2024.
- Yu Sun, Xiaolong Wang, Zhuang Liu, John Miller, Alexei Efros, and Moritz Hardt. Test-time training with self-supervision for generalization under distribution shifts. In International conference on machine learning, pages 9229–9248. PMLR, 2020.
- Sang Michael Xie, Aditi Raghunathan, Percy Liang, and Tengyu Ma. An explanation of in-context learning as implicit bayesian inference. arXiv preprint arXiv:2111.02080, 2021.
- Johannes Von Oswald, Eyvind Niklasson, Maximilian Schlegel, Seijin Kobayashi, Nicolas Zucchet, Nino Scherrer, Nolan Miller, Mark Sandler, Max Vladymyrov, Razvan Pascanu, et al. Uncovering mesa-optimization algorithms in transformers. arXiv preprint arXiv:2309.05858, 2023b.
- Michael Hahn and Navin Goyal. A theory of emergent in-context learning as implicit structure induction. arXiv preprint arXiv:2303.07971, 2023.
- Kwangjun Ahn, Xiang Cheng, Minhak Song, Chulhee Yun, Ali Jadbabaie, and Suvrit Sra. Linear attention is (maybe) all you need (to understand transformer optimization). arXiv preprint arXiv:2310.01082, 2023.
- Angeliki Giannou, Liu Yang, Tianhao Wang, Dimitris Papailiopoulos, and Jason D Lee. How well can transformers emulate in-context newton’s method? arXiv preprint arXiv:2403.03183, 2024.
- Xingwu Chen, Lei Zhao, and Difan Zou. How transformers utilize multi-head attention in in-context learning? a case study on sparse linear regression. arXiv preprint arXiv:2408.04532, 2024.
- Yingqian Cui, Jie Ren, Pengfei He, Jiliang Tang, and Yue Xing. Superiority of multi-head attention in in-context linear regression. arXiv preprint arXiv:2401.17426, 2024. 
- Robert A Jacobs, Michael I Jordan, Steven J Nowlan, and Geoffrey E Hinton. Adaptive mixtures of local experts. Neural computation, 3(1):79–87, 1991.
- Shai Shalev-Shwartz and Shai Ben-David. Understanding machine learning: From theory to algorithms. Cambridge university press, 2014.
- Sara A Geer. Empirical Processes in M-estimation, volume 6. Cambridge university press, 2000.










```
\bibitem[Liu et~al.(2021)Liu, Shen, Zhang, Dolan, Carin, and Chen]{liu2021makes}
Jiachang Liu, Dinghan Shen, Yizhe Zhang, Bill Dolan, Lawrence Carin, and Weizhu Chen.
\newblock What makes good in-context examples for gpt-$3 $?
\newblock \emph{arXiv preprint arXiv:2101.06804}, 2021.

\bibitem[Lu et~al.(2021)Lu, Bartolo, Moore, Riedel, and Stenetorp]{lu2021fantastically}
Yao Lu, Max Bartolo, Alastair Moore, Sebastian Riedel, and Pontus Stenetorp.
\newblock Fantastically ordered prompts and where to find them: Overcoming few-shot prompt order sensitivity.
\newblock \emph{arXiv preprint arXiv:2104.08786}, 2021.

\bibitem[Wei et~al.(2022)Wei, Wang, Schuurmans, Bosma, Xia, Chi, Le, Zhou, et~al.]{wei2022chain}
Jason Wei, Xuezhi Wang, Dale Schuurmans, Maarten Bosma, Fei Xia, Ed~Chi, Quoc~V Le, Denny Zhou, et~al.
\newblock Chain-of-thought prompting elicits reasoning in large language models.
\newblock \emph{Advances in neural information processing systems}, 35:\penalty0 24824--24837, 2022.

\bibitem[Wu et~al.(2022)Wu, Wang, Ye, and Kong]{wu2022self}
Zhiyong Wu, Yaoxiang Wang, Jiacheng Ye, and Lingpeng Kong.
\newblock Self-adaptive in-context learning: An information compression perspective for in-context example selection and ordering.
\newblock \emph{arXiv preprint arXiv:2212.10375}, 2022.

\bibitem[Achiam et~al.(2023)Achiam, Adler, Agarwal, Ahmad, Akkaya, Aleman, Almeida, Altenschmidt, Altman, Anadkat, et~al.]{achiam2023gpt}
Josh Achiam, Steven Adler, Sandhini Agarwal, Lama Ahmad, Ilge Akkaya, Florencia~Leoni Aleman, Diogo Almeida, Janko Altenschmidt, Sam Altman, Shyamal Anadkat, et~al.
\newblock Gpt-4 technical report.
\newblock \emph{arXiv preprint arXiv:2303.08774}, 2023.

\bibitem[Touvron et~al.(2023)Touvron, Lavril, Izacard, Martinet, Lachaux, Lacroix, Rozi{\`e}re, Goyal, Hambro, Azhar, et~al.]{touvron2023llama}
Hugo Touvron, Thibaut Lavril, Gautier Izacard, Xavier Martinet, Marie-Anne Lachaux, Timoth{\'e}e Lacroix, Baptiste Rozi{\`e}re, Naman Goyal, Eric Hambro, Faisal Azhar, et~al.
\newblock Llama: Open and efficient foundation language models.
\newblock \emph{arXiv preprint arXiv:2302.13971}, 2023.

\bibitem[Dai et~al.(2022)Dai, Sun, Dong, Hao, Ma, Sui, and Wei]{dai2022can}
Damai Dai, Yutao Sun, Li~Dong, Yaru Hao, Shuming Ma, Zhifang Sui, and Furu Wei.
\newblock Why can gpt learn in-context? language models implicitly perform gradient descent as meta-optimizers.
\newblock \emph{arXiv preprint arXiv:2212.10559}, 2022.

\bibitem[Von~Oswald et~al.(2023{\natexlab{a}})Von~Oswald, Niklasson, Randazzo, Sacramento, Mordvintsev, Zhmoginov, and Vladymyrov]{von2023transformers}
Johannes Von~Oswald, Eyvind Niklasson, Ettore Randazzo, Jo{\~a}o Sacramento, Alexander Mordvintsev, Andrey Zhmoginov, and Max Vladymyrov.
\newblock Transformers learn in-context by gradient descent.
\newblock In \emph{International Conference on Machine Learning}, pages 35151--35174. PMLR, 2023{\natexlab{a}}.

\bibitem[Garg et~al.(2022)Garg, Tsipras, Liang, and Valiant]{garg2022can}
Shivam Garg, Dimitris Tsipras, Percy~S Liang, and Gregory Valiant.
\newblock What can transformers learn in-context? a case study of simple function classes.
\newblock \emph{Advances in Neural Information Processing Systems}, 35:\penalty0 30583--30598, 2022.

\bibitem[Aky{\"u}rek et~al.(2022)Aky{\"u}rek, Schuurmans, Andreas, Ma, and Zhou]{akyurek2022learning}
Ekin Aky{\"u}rek, Dale Schuurmans, Jacob Andreas, Tengyu Ma, and Denny Zhou.
\newblock What learning algorithm is in-context learning? investigations with linear models.
\newblock \emph{arXiv preprint arXiv:2211.15661}, 2022.

\bibitem[Mahankali et~al.(2023)Mahankali, Hashimoto, and Ma]{mahankali2023one}
Arvind Mahankali, Tatsunori~B Hashimoto, and Tengyu Ma.
\newblock One step of gradient descent is provably the optimal in-context learner with one layer of linear self-attention.
\newblock \emph{arXiv preprint arXiv:2307.03576}, 2023.

\bibitem[Ahn et~al.(2024)Ahn, Cheng, Daneshmand, and Sra]{ahn2024transformers}
Kwangjun Ahn, Xiang Cheng, Hadi Daneshmand, and Suvrit Sra.
\newblock Transformers learn to implement preconditioned gradient descent for in-context learning.
\newblock \emph{Advances in Neural Information Processing Systems}, 36, 2024.

\bibitem[Fu et~al.(2023)Fu, Chen, Jia, and Sharan]{fu2023transformers}
Deqing Fu, Tian-Qi Chen, Robin Jia, and Vatsal Sharan.
\newblock Transformers learn higher-order optimization methods for in-context learning: A study with linear models.
\newblock \emph{arXiv preprint arXiv:2310.17086}, 2023.

\bibitem[Vladymyrov et~al.(2024)Vladymyrov, Von~Oswald, Sandler, and Ge]{vladymyrov2024linear}
Max Vladymyrov, Johannes Von~Oswald, Mark Sandler, and Rong Ge.
\newblock Linear transformers are versatile in-context learners.
\newblock \emph{arXiv preprint arXiv:2402.14180}, 2024.

\bibitem[Goh(2017)]{goh2017why}
Gabriel Goh.
\newblock Why momentum really works.
\newblock \emph{Distill}, 2017.
\newblock \doi{10.23915/distill.00006}.
\newblock URL \url{http://distill.pub/2017/momentum}.

\bibitem[Wu et~al.(2020)Wu, Lan, Qian, Gu, Geramifard, and Yu]{wu2020Memformer}
Qingyang Wu, Zhenzhong Lan, Kun Qian, Jing Gu, Alborz Geramifard, and Zhou Yu.
\newblock Memformer: A memory-augmented transformer for sequence modeling.
\newblock \emph{arXiv preprint arXiv:2010.06891}, 2020.

\bibitem[Xu et~al.(2021)Xu, Liang, Cheng, Wei, Chen, and Zhang]{xu2021transformer}
Dongkuan Xu, Junjie Liang, Wei Cheng, Hua Wei, Haifeng Chen, and Xiang Zhang.
\newblock Transformer-style relational reasoning with dynamic memory updating for temporal network modeling.
\newblock In \emph{Proceedings of the AAAI conference on artificial intelligence}, volume~35, pages 4546--4554, 2021.

\bibitem[Zhang et~al.(2024)Zhang, Frei, and Bartlett]{zhang2024trained}
Ruiqi Zhang, Spencer Frei, and Peter~L Bartlett.
\newblock Trained transformers learn linear models in-context.
\newblock \emph{Journal of Machine Learning Research}, 25\penalty0 (49):\penalty0 1--55, 2024.

\bibitem[Schlag et~al.(2021)Schlag, Irie, and Schmidhuber]{schlag2021linear}
Imanol Schlag, Kazuki Irie, and J{\"u}rgen Schmidhuber.
\newblock Linear transformers are secretly fast weight programmers.
\newblock In \emph{International Conference on Machine Learning}, pages 9355--9366. PMLR, 2021.

\bibitem[Snell et~al.(2024)Snell, Lee, Xu, and Kumar]{snell2024scaling}
Charlie Snell, Jaehoon Lee, Kelvin Xu, and Aviral Kumar.
\newblock Scaling llm test-time compute optimally can be more effective than scaling model parameters.
\newblock \emph{ICLR 2025 arXiv:2408.03314}, 2024.

\bibitem[Sun et~al.(2020)Sun, Wang, Liu, Miller, Efros, and Hardt]{sun2020test}
Yu~Sun, Xiaolong Wang, Zhuang Liu, John Miller, Alexei Efros, and Moritz Hardt.
\newblock Test-time training with self-supervision for generalization under distribution shifts.
\newblock In \emph{International conference on machine learning}, pages 9229--9248. PMLR, 2020.

\bibitem[Xie et~al.(2021)Xie, Raghunathan, Liang, and Ma]{xie2021explanation}
Sang~Michael Xie, Aditi Raghunathan, Percy Liang, and Tengyu Ma.
\newblock An explanation of in-context learning as implicit bayesian inference.
\newblock \emph{arXiv preprint arXiv:2111.02080}, 2021.

\bibitem[Von~Oswald et~al.(2023{\natexlab{b}})Von~Oswald, Niklasson, Schlegel, Kobayashi, Zucchet, Scherrer, Miller, Sandler, Vladymyrov, Pascanu, et~al.]{von2023uncovering}
Johannes Von~Oswald, Eyvind Niklasson, Maximilian Schlegel, Seijin Kobayashi, Nicolas Zucchet, Nino Scherrer, Nolan Miller, Mark Sandler, Max Vladymyrov, Razvan Pascanu, et~al.
\newblock Uncovering mesa-optimization algorithms in transformers.
\newblock \emph{arXiv preprint arXiv:2309.05858}, 2023{\natexlab{b}}.

\bibitem[Hahn and Goyal(2023)]{hahn2023theory}
Michael Hahn and Navin Goyal.
\newblock A theory of emergent in-context learning as implicit structure induction.
\newblock \emph{arXiv preprint arXiv:2303.07971}, 2023.

\bibitem[Ahn et~al.(2023)Ahn, Cheng, Song, Yun, Jadbabaie, and Sra]{ahn2023linear}
Kwangjun Ahn, Xiang Cheng, Minhak Song, Chulhee Yun, Ali Jadbabaie, and Suvrit Sra.
\newblock Linear attention is (maybe) all you need (to understand transformer optimization).
\newblock \emph{arXiv preprint arXiv:2310.01082}, 2023.

\bibitem[Giannou et~al.(2024)Giannou, Yang, Wang, Papailiopoulos, and Lee]{giannou2024well}
Angeliki Giannou, Liu Yang, Tianhao Wang, Dimitris Papailiopoulos, and Jason~D Lee.
\newblock How well can transformers emulate in-context newton's method?
\newblock \emph{arXiv preprint arXiv:2403.03183}, 2024.

\bibitem[Chen et~al.(2024)Chen, Zhao, and Zou]{chen2024transformers}
Xingwu Chen, Lei Zhao, and Difan Zou.
\newblock How transformers utilize multi-head attention in in-context learning? a case study on sparse linear regression.
\newblock \emph{arXiv preprint arXiv:2408.04532}, 2024.

\bibitem[Cui et~al.(2024)Cui, Ren, He, Tang, and Xing]{cui2024superiority}
Yingqian Cui, Jie Ren, Pengfei He, Jiliang Tang, and Yue Xing.
\newblock Superiority of multi-head attention in in-context linear regression.
\newblock \emph{arXiv preprint arXiv:2401.17426}, 2024.

\bibitem[Jacobs et~al.(1991)Jacobs, Jordan, Nowlan, and Hinton]{jacobs1991adaptive}
Robert~A Jacobs, Michael~I Jordan, Steven~J Nowlan, and Geoffrey~E Hinton.
\newblock Adaptive mixtures of local experts.
\newblock \emph{Neural computation}, 3\penalty0 (1):\penalty0 79--87, 1991.

\bibitem[Shalev-Shwartz and Ben-David(2014)]{shalev2014understanding}
Shai Shalev-Shwartz and Shai Ben-David.
\newblock \emph{Understanding machine learning: From theory to algorithms}.
\newblock Cambridge university press, 2014.

\bibitem[Geer(2000)]{geer2000empirical}
Sara~A Geer.
\newblock \emph{Empirical Processes in M-estimation}, volume~6.
\newblock Cambridge university press, 2000.

\end{thebibliography}
```