---
aliases: 
anki: false
created: 2024-07-02 19:11
parent:
  - "[[Relation]]"
connected:
  - "[[Ternary operation]]"
tags: []
---

> [!tip] 
Тернарное отношение $\mathcal{R}$ на множестве $\mathcal{A}$ 
это подмножество $\mathcal{R} \subseteq \mathcal{A} \times \mathcal{A} \times \mathcal{A}$.


**Тернарное отношение** на множестве $\mathcal{A}$ – это подмножество декартова произведения $\mathcal{A} \times \mathcal{A} \times \mathcal{A}$. Тернарное отношение связывает тройки элементов множества определенным способом.



**Примеры:**
- **Упорядоченность тройки**: $(x, y, z) \in \mathcal{R}$ может означать, что $x \leq y \leq z$.
- **Коллинеарность точек**: В геометрии тернарное отношение может описывать коллинеарность трех точек на плоскости. $(A, B, C) \in \mathcal{R}$ означает, что точки $A$, $B$ и $C$ лежат на одной прямой.



### Ключевые различия между тернарными операциями и тернарными отношениями

1. **Назначение**:
   - **Тернарная операция**: Описывает правило комбинирования трех элементов множества для получения одного элемента того же множества.
   - **Тернарное отношение**: Описывает отношение между тремя элементами множества, указывая, обладают ли они некоторым свойством.

2. **Результат**:
   - **Тернарная операция**: Возвращает один элемент того же множества.
   - **Тернарное отношение**: Возвращает логическое значение (истина или ложь) для каждой тройки элементов.

3. **Структура**:
   - **Тернарная операция**: Функция, определяющая преобразование тройки элементов множества.
   - **Тернарное отношение**: Подмножество множества троек, определяющее, какие тройки элементов обладают данным свойством.

### Примеры и пояснения

- **Тернарная операция**: Пусть $\mathcal{A} = \mathbb{R}$ (множество вещественных чисел). Тернарная операция $f : \mathcal{A} \times \mathcal{A} \times \mathcal{A} \to \mathcal{A}$ определяется как $f(x, y, z) = x + y + z$. Например, если $x = 1$, $y = 2$ и $z = 3$, то $f(x, y, z) = 1 + 2 + 3 = 6$.

- **Тернарное отношение**: Пусть $\mathcal{A} = \mathbb{R}$ (множество вещественных чисел). Тернарное отношение $\mathcal{R} \subseteq \mathcal{A} \times \mathcal{A} \times \mathcal{A}$ определяется как множество упорядоченных троек, таких что первая координата меньше второй, а вторая меньше третьей. То есть $\mathcal{R} = \{(x, y, z) \mid x \leq y \leq z\}$. Например, $(1, 2, 3) \in \mathcal{R}$ (упорядоченная тройка), а $(3, 2, 1) \notin \mathcal{R}$ (неупорядоченная тройка).
