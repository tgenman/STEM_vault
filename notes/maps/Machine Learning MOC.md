---
aliases:
  - ML MOC
  - 004.8 Машинное обучение
  - ML
  - 004.85 Machine Learning (notion)
tags:
  - контент/мос
connected:
  - "[[004.432.2 🐍 Python MOC]]"
  - "[[Neural Networks (notion)]]"
parent:
  - "[[004 IT MOC]]"
  - "[[004. 8 AI MOC]]"
created: 2023-07-31 18:35
updated: 2026-09-13
---
# machine learning

Карта задач, методов и основных понятий машинного обучения.

## учебные материалы

- [[1.3. Машинное обучение]] — конспект, FAQ, вопросы и глоссарий; точный первоисточник не установлен.

### экзаменационные материалы

Исходные названия без приложенных материалов; актуальность не уточнена.

- Machine Learning exam questions-answers
- Machine Learning exam Theoretical minimum

## направления

- NLP
- [[notes/_meta/moc/Computer Vision|CV]]
- [[Reinforcement Learning|RL]]

## основные понятия

- [[Feature Representation]]
- [[representation learning]]

Method = [[Model (ML)]] + [[Loss function|Criterion]]  + [[Algorithm of learning]]


[[Эпоха]]

- [[Linear models]]
    - [[Linear models#мультиколлинеарность]] — сохранённое пояснение.
[[Интерпретируемость]]

[[Hyperparameter]]

[[Parameter]]

Cross-validation
[[Underfitting]],
[[Overfitting]],
training stage,  validation stage, testing stage
[[Training Dataset]]
regularization


## данные, обучение и оценка

- [[Object (ML)]]
- [[Features]]
- [[Labels]]
- [[краудсорсинг]]
- [[Data drift]]
- [[Concept drift]]


- [[Loss function]]
    - [[Mean absolute error]]
    - [[квадратичная потеря в линейной регрессии]] — сохранённое объяснение и формулы.
    - [[Mean absolute percentage error]]
    - [[Log loss]] - Логарифмические потери тесно связаны с концепцией [[Кросс-энтропия]]
    - [[Huber loss]]


-  [[Gradient Descent]]
    - [[Stochastic gradient descent]]
    - [[Mini-batch gradient descent]]
    - [[Batch gradient descent]]


- [[Activation function]] активация нейрона. Вносит нелинейность
    - Ступенчатая функция
    - [[Sigmoid function]]


- [[Метрика качества]]
    - [[бизнес-метрики]]
    - [[Online метрики]]
    - [[Offline метрики]]

    - [[Confusion matrix]]
        - [[False positive]], [[False negative]]
        - [[True positive]], [[True negative]]
        - [[Accuracy]],  [[Error rate]]
        - [[Precision]], [[Recall]], [[F1-measure]]
        - [[Recall|True positive rate TPR]] , [[False positive rate FPR]], [[ROC curve]],
            - [[AUC ROC]]
        - «Полнота — это чувствительность, но точность и избирательность — разные вещи».


“receiver operating characteristic (ROC) curve.”


---

## по задачам
- [[Regression (machine learning)]]
- [[Classification]]
    - [[Binary classification]]
    - [[Multiclass classification]]
    - [[Multilabel classification]]
- [[Ranking]]
- image segmentation
- machine translation
- generative models, which aim to create new, plausible objects.

## по типам алгоритмов

- [[self-supervised learning]]
- [[Supervised Learning]] (есть заданная выборка, есть учитель)
    -  [[Classification ML]]
        - binary classification
        - multiclass classification
        - multilabel classification
        - [[Naive Bayes]]
        - [[Decision trees]]
        - [Логистическая Регрессия](https://ru.wikipedia.org/wiki/%D0%9B%D0%BE%D0%B3%D0%B8%D1%81%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B0%D1%8F_%D1%80%D0%B5%D0%B3%D1%80%D0%B5%D1%81%D1%81%D0%B8%D1%8F) Logistic regression
        - [K-ближайших соседей](https://ru.wikipedia.org/wiki/%D0%9C%D0%B5%D1%82%D0%BE%D0%B4_k-%D0%B1%D0%BB%D0%B8%D0%B6%D0%B0%D0%B9%D1%88%D0%B8%D1%85_%D1%81%D0%BE%D1%81%D0%B5%D0%B4%D0%B5%D0%B9) K-NN
        - [[Support Vector Machine (SVM)]]
    - [[Regression (machine learning)]]
        - Linear regression
        - Polynomial regression
        - [[Linear and Polynomial Regression]]
        - Ridge-Lasso Regression
    - [[Ranking]]
- [[Unsupervised Learning]] (есть заданная выборка, нет учителя)
    - [[Clustering (machine learning)]]
    - [[Поиск правил (ассоциация)]]
    - [[Dimension reduction (generalization)]]
    - Генеративные алгоритмы
        - GAN
- [[Reinforcement Learning]] (нет заданной выборки, есть фидбек среды)
- [[Ensemble Methods]]
    - [[Стейкинг (ансамблевые методы)]]
    - [[Беггинг (ансамблевые методы)]]
    - [[Бустинг (ансамблевые методы)]]
- [[Neural Networks (notion)]]
    - [[Convolutional neural network]] (CNN)
    - [[Recurrent Neural Network]] (RNN)
    - [[Generative Adversarial Networks]] (GAN)
    - [[Autoencoders]]
    - [[Multilayer percepton]] (MLP)


![[Pasted image 20240611102506.png]]


---

## разные ссылки

[Объяснения от гугла про разные аспекты машинного обучения](https://pair.withgoogle.com/explorables/)
[Essential Guide to keep up with AI/ML/DL/CV](https://github.com/BAILOOL/DoYouEvenLearn/blob/master/README.md)


---

![[Pasted image 20230503092745.png|330]] ![[Pasted image 20230503092845.png|330]]


![[BED72584-D248-42EF-803E-16C6878D5607.jpeg]]

## сохранённые пояснения

Фрагменты прежнего оглавления; происхождение и содержательная корректность ещё не проверены.


для решения большинства практических задач на сегодня достаточно знать только два типа моделей — **градиентный бустинг на решающих деревьях** и **нейросетевые модели**

---

### пометка о MSE и RMSE

Сохранённая строка прежней карты; смысл связи не уточнён:

[[Mean squared error]] Root Mean S E [[Standard deviation]]
