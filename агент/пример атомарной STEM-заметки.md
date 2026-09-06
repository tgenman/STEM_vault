---
tags:
created: 2026-08-28
updated: 2026-09-06
---
# пример атомарной STEM-заметки

Это полный образец новой понятийной заметки с карточкой Anki. Он показывает совместную структуру элементов, но не заменяет `templates/УН (template).md`, локальный MOC, источник и актуальный протокол [[агент/Anki]].

## обязательный каркас

- Frontmatter содержит только применимые свойства и фактические связи.
- Определение математически точно задаёт объект, параметры и условия применимости.
- Формула вынесена из callout определения и использует принятые в исходном Markdown разделители.
- Пример иллюстрирует именно сформулированное определение.
- Если добавлена карточка, `anki: true`, колода и модель актуальны, а у новой карточки нет вручную заданного `ID`.

## полный пример

```markdown
---
aliases:
  - Размещение без повторений
  - Расстановки без повторений
anki: true
created: 2026-08-28
parent:
  - "[[519.101 Combinatorics MOC]]"
connected:
  - "[[Factorial]]"
  - "[[Tuple]]"
  - "[[Arrangements with repetition]]"
tags:
  - контент/определение
---

> [!tip] An arrangement without repetition $A_n^k$
> An arrangement without repetition of $k$ elements from an $n$-element set $A$ is an ordered $k$-[[Tuple|tuple]] $(x_1,\ldots,x_k)$ of pairwise distinct elements of $A$, where $0 \le k \le n$.

$$
A_n^k = \frac{n!}{(n-k)!} = n(n-1)\cdots(n-k+1)
$$

## example

If three books are chosen and arranged from five distinct books, then

$$
A_5^3 = \frac{5!}{(5-3)!} = 60.
$$

## Anki

TARGET DECK: stem::math::combinatorics
START
math_complex
FRONT: Arrangements without repetition
BACK: An ordered $k$-tuple of pairwise distinct elements chosen from an $n$-element set, where $0 \le k \le n$.
FORMULA: $A_n^k = \frac{n!}{(n-k)!}$
PICTURE:
ADDITIONAL: Order matters; elements cannot repeat.
PROOF:
END
```

## вариативные части

- `aliases`, `parent`, `connected` и `tags` заполняются по фактической заметке; значения из примера не копируются автоматически.
- Разделы с доказательством, изображением, дополнительными свойствами или контрпримером добавляются только при наличии содержания.
- Если в теле заметки нужно изображение, используй `![[attachment.png|300]]`; в поле карточки — `PICTURE: ![[attachment.png]]`.
- Тип карточки выбирается по проверяемой единице знания. `math_complex` из примера не является универсальным значением по умолчанию.
- Если карточки нет, раздел Anki отсутствует, а для обычной понятийной заметки используется `anki: false`. В MOC поле `anki` опускается.
