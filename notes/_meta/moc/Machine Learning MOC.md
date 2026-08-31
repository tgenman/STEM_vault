---
aliases:
  - ML MOC
tags:
  - content/moc
connected:
  - "[[004.432.2 🐍 Python MOC]]"
  - "[[Neural Networks (notion)]]"
parent:
  - "[[004.85 Machine Learning (notion)]]"
  - "[[004. 8 AI MOC]]"
---
- [[yandex course - ML (temp)]]

- NLP
- [[notes/_meta/moc/Computer Vision|CV]]
- [[Reinforcement Learning|RL]]

Method = [[Model (ML)]] + [[Loss function|Criterion]]  + [[Algorithm of learning]]


 **краудсорсинга**, то есть привлечение людей, готовых разметить много данных.
**citizen science** – разметку данных волонтёрами без какого-либо вознаграждения

Подходы, связанные с использованием неразмеченных данных для решения задач обучения с учителем, объединяются термином **self-supervised learning** и очень активно используются сейчас. 
Важной составляющей является **обучение представлений** (**representation learning**) — задача построения компактных векторов небольшой размерности из сложных по структуре данных, например, изображений, звука, текстов, графов, так, чтобы близкие по структуре или семантике данные получали метрически близкие представления

- **Data drift**. С течением времени данные могут меняться. Например, может измениться схема сбора данных, и они начнут приходить в формате, который вообще не обрабатывается моделью. Или же может поменяться распределение данных: скажем, если вы делали образовательный сервис для студентов, а к вам стали приходить и более зрелые люди. Data drift – это суровая реальность для любой системы, которая решает не сиюминутную задачу, поэтому нужно уметь мониторить распределение данных и, если нужно, обновлять модель.
- **concept drift** — изменение зависимости между признаками и таргетом. Например, если вы делаете музыкальные рекомендации, вам нужно будет учитывать и появление новых треков, и изменение вкусов аудитории.

для решения большинства практических задач на сегодня достаточно знать только два типа моделей — **градиентный бустинг на решающих деревьях** и **нейросетевые модели**

---

Функция потерь $ \frac{1}{N} \sum_{i=1}^{N} (y_{i} - \langle x_{i}, w \rangle)^{2} $ называется Mean Squared Error, MSE или среднеквадратическим отклонением. Разница с $ L^{2} $-нормой чисто косметическая, на алгоритм решения задачи она не влияет: 

$$ \text{MSE}(f, X, y) = \frac{1}{N} \| y - Xw \|_{2}^{2} $$ 

В самом широком смысле, функции работают с объектами множеств: берут какой-то входящий объект из одного множества и выдают на выходе соответствующий ему объект из другого. Если мы имеем дело с отображением, которое на вход принимает функции, а на выходе выдаёт число, то такое отображение называют функционалом. Если вы посмотрите на нашу функцию потерь, то увидите, что это именно функционал. Для каждой конкретной линейной функции, которую задают веса $ w_{i} $, мы получаем число, которое оценивает, насколько точно эта функция приближает наши значения $ y $. Чем меньше это число, тем точнее наше решение, значит для того, чтобы найти лучшую модель, этот функционал нам надо минимизировать по $ w $: 

$$ \| y - Xw \|_{2}^{2} \rightarrow \min_{w} $$ 

Эту задачу можно решать разными способами. В этом параграфе мы сначала решим эту задачу аналитически, а потом приближенно. Сравнение двух этих решений позволит нам проиллюстрировать преимущества того подхода, которому посвящена эта книга. На наш взгляд, это самый простой способ "на пальцах" показать суть машинного обучения.

---

Конечно, в жизни редко бывает так, что признаки строго линейно зависимы, а вот быть приближённо линейно зависимыми они вполне могут быть. Такая ситуация называется **мультиколлинеарностью**.

---


[[Эпоха]]

[[Linear models]]
[[Интерпретируемость]]

Hyperparameter
Any quantity that you set before the training process .

Parameter
Any quantity that the model creates or modifies during the training process

Cross-validation
[[Underfitting]], 
[[Overfitting]], 
training stage,  validation stage, testing stage
[[Training Dataset]]
regularization


- [[Object (ML)]]
- [[Features]]
- [[Labels]]


- [[Loss function]]
    - [[Mean absolute error]] 
    - [[Mean squared error]] Root Mean S E [[Standard deviation]]
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

### По задачам
- [[Regression (machine learning)]]
- [[Classification]]
    - [[Binary classification]]
    - [[Multiclass classification]]
    - [[Multilabel classification]]
- [[Ranking]]
- image segmentation
- machine translation
- generative models, which aim to create new, plausible objects.

### По типам алгоритмов
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

#### Разные ссылки

[Объяснения от гугла про разные аспекты машинного обучения](https://pair.withgoogle.com/explorables/)
[Essential Guide to keep up with AI/ML/DL/CV](https://github.com/BAILOOL/DoYouEvenLearn/blob/master/README.md)


---

![[Pasted image 20230503092745.png|330]] ![[Pasted image 20230503092845.png|330]]



![[BED72584-D248-42EF-803E-16C6878D5607.jpeg]]
