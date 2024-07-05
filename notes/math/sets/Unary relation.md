---
aliases:
  - Унарное отношение
publish: true
anki: false
created: 2024-07-02 19:11
parent:
  - "[[Relation on elements of sets]]"
connected:
  - "#обс/linking"
tags: []
---

> [!tip] Унарное отношение $\mathcal{P}$ на множестве $\mathcal{A}$ 
это подмножество $\mathcal{P} \subseteq \mathcal{A}$.


**Унарное отношение** на множестве $\mathcal{A}$ – это подмножество $\mathcal{A}$. Унарное отношение указывает на то, обладает ли элемент определенным свойством.

Примеры:
- **Четность**: $\mathcal{P} = \{x \in \mathbb{Z} \mid x \; \text{четное}\}$.
- **Положительность**: $\mathcal{P} = \{x \in \mathbb{R} \mid x > 0\}$.


### Ключевые различия между унарными операциями и унарными отношениями

1. **Назначение**:
   - **Унарная операция**: Описывает правило преобразования одного элемента множества в другой элемент того же множества.
   - **Унарное отношение**: Описывает свойство, которым элемент либо обладает, либо нет.

2. **Результат**:
   - **Унарная операция**: Возвращает элемент того же множества.
   - **Унарное отношение**: Возвращает логическое значение (обычно рассматривается как подмножество элементов, обладающих определенным свойством).

3. **Структура**:
   - **Унарная операция**: Функция, определяющая преобразование элементов множества.
   - **Унарное отношение**: Подмножество множества, определяющее, какие элементы обладают данным свойством.

### Примеры и пояснения

- **Унарная операция**: Пусть $\mathcal{A} = \mathbb{Z}$ (множество целых чисел). Унарная операция $-: \mathcal{A} \to \mathcal{A}$ определяется как $-x$, где $x \in \mathcal{A}$. Например, если $x = 5$, то унарная операция $-x$ возвращает $-5$.

- **Унарное отношение**: Пусть $\mathcal{A} = \mathbb{Z}$ (множество целых чисел). Унарное отношение $\mathcal{P} \subseteq \mathcal{A}$ определяется как множество четных чисел. То есть $\mathcal{P} = \{x \in \mathcal{A} \mid x \; \text{четное}\}$. Например, $4 \in \mathcal{P}$ (четное число) и $5 \notin \mathcal{P}$ (нечетное число).