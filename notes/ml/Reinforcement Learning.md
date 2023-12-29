---
aliases: Обучение с подкреплением
publish: true
created: 2023-05-03 21:35
---

«Брось робота в лабиринт и пусть ищет выход»

Цель — **минимизировать ошибки, а не рассчитать все ходы**.
![[Pasted image 20230503213749.png|300]]
Сегодня используют для:
-   Самоуправляемых автомобилей
-   Роботов пылесосов
-   Игр
-   Автоматической торговли
-   Управления ресурсами предприятий

Популярные алгоритмы:
[Q-Learning](https://ru.wikipedia.org/wiki/Q-%D0%BE%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5), 
[SARSA](https://en.wikipedia.org/wiki/State%E2%80%93action%E2%80%93reward%E2%80%93state%E2%80%93action), 
DQN, 
[A3C](https://medium.com/emergent-future/simple-reinforcement-learning-with-tensorflow-part-8-asynchronous-actor-critic-agents-a3c-c88f72a5e9f2), 
[Генетический Алгоритм](https://ru.wikipedia.org/wiki/%D0%93%D0%B5%D0%BD%D0%B5%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D0%B9_%D0%B0%D0%BB%D0%B3%D0%BE%D1%80%D0%B8%D1%82%D0%BC)

В обучении с подкреплением **машина не запоминает каждое движение, а пытается обобщить ситуации, чтобы выходить из них с максимальной выгодой**

![[Pasted image 20230503214052.png]]
Эта идея лежит в основе алгоритма [Q-learning](https://www.youtube.com/watch?v=aCEvtRtNO-M) и его производных (SARSA и DQN). Буква Q в названии означает слово Quality, то есть робот учится поступать наиболее качественно в любой ситуации, а все ситуации он запоминает как простой [марковский процесс](https://ru.wikipedia.org/wiki/%D0%9C%D0%B0%D1%80%D0%BA%D0%BE%D0%B2%D1%81%D0%BA%D0%B8%D0%B9_%D0%BF%D1%80%D0%BE%D1%86%D0%B5%D1%81%D1%81).

![[Pasted image 20230503214209.png]]
 Другие идут глубже и отдают эту работу нейросетям, пусть сами всё найдут. Так вместо Q-learning'а у нас появляется Deep Q-Network (DQN).




**Connected with:**
- subtype of [[Machine Learning MOC]]



