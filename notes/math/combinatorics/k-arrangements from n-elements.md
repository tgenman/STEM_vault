---
aliases:
  - Pазме­щение из n элементов по k
publish: true
anki: true
parent:
  - "[[519.101 Combinatorics]]"
created: 2023-10-23 16:47
connected:
  - "[[Factorial]]"
  - "[[Tuple]]"
  - "[[k-combination from n elements]]"
---
arrangement - расстановка, размещение
permutation - перестановка ${} k = n$

Let ${} k \leq n$  and $A = \set{a_1,..., a_n}$ be a finite set

An ==arrangement== of $n {}$ elements (of the set $A {}$) is an ordered $n$-[[Tuple|tuple]] $(x_1,..., x_n) {}$ elements of $A$, where each elements occurs exactly once

[[Permutation of n elements]]

### No repetition (число k-размещений без повторений из n объектов):
$$A_n^k= V_{n, k} = \frac{n!}{(n-k)!} = n \cdot (n-1) \cdot ... \cdot (n - k + 1)$$

### With repetition (число k-размещений c повторениями из n объектов):
если число видов элементов равно $n$, а число мест равно $k$,
$$
\bar{A_n^k} = n \cdot n \cdot ... \cdot n = n^k
$$
$$
\bar{A_n^n} = n \cdot n \cdot ... \cdot n = n^n
$$
Синонимы: [[Vector]] [[Tuple]]


> [!info]+
> ```dataview 
> TABLE without id
> map(file.outlinks, (link) => "[[" + meta(link).path + "]]") AS "Исходящие",
> map(file.inlinks, (link) => "[[" + meta(link).path + "]]") AS "Входящие"
> WHERE file.name = this.file.name
> ```



### Anki
TARGET DECK: Math::Combinatorics
START
Math def
Title_eng:  k-arrangements from n-elements (No repetition)
Title_rus:  число k-размещений без повторений из n объектов
Description_eng: is an ordered n-tuple ${} (x_1,..., x_n)$ elements of A, where each elements occurs exactly once
Description_rus:
Formula_main: $$
A_n^k= V_{n, k} = \frac{n!}{(n-k)!} = n \cdot (n-1) \cdot ... \cdot (n - k + 1)
$$
Formula_additional:
<!--ID: 1698069638670-->
END

START
Math def
Title_eng:  k-arrangements from n-elements (With repetition)
Title_rus:  число k-размещений c повторениями из n объектов
Description_eng:  is an ordered n-tuple $(x_1,..., x_n)$ elements of A, where each elements occurs any times
Description_rus:
Formula_main: $$
\bar{A_n^k} = n \cdot n \cdot ... \cdot n = n^k
$$
Formula_additional:
<!--ID: 1698069774907-->
END


Вы абсолютно правы, я сделал ошибку в анализе первого случая. Давайте пересмотрим решение.

Задача состоит в том, чтобы выбрать 6 карт так, чтобы были представлены все четыре масти. Возможные способы распределения мастей среди этих 6 карт:

1. **Случай 1**: 2 карты одной масти, 2 карты другой масти, 1 карта третьей масти и 1 карта четвертой масти.
2. **Случай 2**: 3 карты одной масти, 1 карта каждой из трех других мастей.

Теперь давайте рассчитаем количество способов для каждого случая:

1. **Для случая 2-2-1-1**:
    
    - Выбираем две масти из четырех для двух карт: $\binom{4}{2}$ способов.
    - Выбираем две карты из каждой из этих двух мастей: $\binom{8}{2} \times \binom{8}{2}$ способов.
    - Выбираем по одной карте из оставшихся двух мастей: $\binom{8}{1} \times \binom{8}{1}$ способов.
2. **Для случая 3-1-1-1**:
    
    - Выбираем одну масть из четырех для трех карт: $\binom{4}{1}$ способов.
    - Выбираем три карты из этой масти: $\binom{8}{3}$ способов.
    - Выбираем по одной карте из каждой из оставшихся трех мастей: $\binom{8}{1} \times \binom{8}{1} \times \binom{8}{1}$ способов.

Теперь выполним расчеты для этих случаев:

Исправленное общее количество способов выбрать 6 карт из колоды из 32 карт так, чтобы среди выбранных карт были представлены все четыре масти, составляет 415,744 способа.

Это число получается путём суммирования количества способов для двух различных случаев распределения карт по мастям: один случай, когда мы выбираем 2 карты каждой из двух мастей и по одной карте для оставшихся двух мастей (2-2-1-1), и другой случай, когда мы выбираем 3 карты одной масти и по одной карте каждой из трёх других мастей (3-1-1-1).

Благодарю за ваше терпение и за то, что указали на ошибку. Если у вас есть ещё вопросы или нужно дополнительное объяснение, пожалуйста, обращайтесь!​
