---
created: 2026-03-02 10:49
tags:
  - content/summary
---

# План фиксов: линейная алгебра (`notes/math/algebra/linal/`)

## Контекст

- `Vault Analysis 2026-02.md`
- `Migration links Analysis.md`
- `AGENTS.md` (правило: `anki` отсутствует для MOC/umbrella)

## Скоуп

Внутри этого плана:

- `notes/math/algebra/linal/` (52 заметки)

Вне скоупа (пока):

- перенос/рефакторинг заметок из `notes/_inbox/` (кроме уже находящихся в `linal/`)
- переименование файлов (делать только через Obsidian UI, чтобы обновились ссылки)

## Цели

- Привести `linal/` к единому мета-формату: убрать legacy `links:` (gap-zone), заполнить `parent`/`connected`, убрать `#обс/linking`.
- Сделать долги честными: `fix/empty` оставлять только там, где реально нет минимального содержания.
- Отделить механику (схема/ссылки) от смысла (мат. корректность) и от Anki (экспорт), чтобы не ломать пайплайн.
- Выделить перегруженные заметки и разбить их по single responsibility.

## Definition of done (Level 1)

Entity/concept заметка:

- Валидный YAML frontmatter: `aliases`, `parent`, `connected`, `created`, `anki`, `tags`.
- В начале тела заметки: `> [!tip] ...` и следующая строка определения тоже начинается с `>`.
- Нет `fix/empty` и нет `#обс/linking`.
- Нет legacy `links:` (gap-zone) и других полей вне YAML.
- Формулы только `$...$`/`$$...$$` (без `\(...\)`).

MOC/зонтичная перечислительная заметка:

- Валидный YAML frontmatter: `aliases`, `parent`, `connected`, `created`, `tags`.
- Поле `anki` отсутствует.
- Тело заметки может быть чистым индексом без определения.

## Снимок состояния (сейчас)

Срез по `notes/math/algebra/linal/`:

- Файлов: 52
- Legacy `links:`: 3
- `fix/empty`: 17
- `#обс/linking`: 14
- Нет YAML frontmatter: 1 (`notes/math/algebra/linal/Linearity.md` — 0 байт)
- Отсутствует `created`: 5
- Отсутствует `parent`: 5
- Отсутствует `connected`: 7
- Отсутствует `tags`: 19
- Отсутствует `anki`: 10 (но часть из них должна остаться без `anki`, т.к. это MOC/umbrella)

Anki/экспорт:

- Legacy тип карточки `Math_TWO_side`: 7 заметок
- `TARGET DECK: math::linal` используется; `stem::math::linal` в папке не встречается

## Инварианты (KISS)

### `parent`

- Для entity/concept заметок внутри `linal/`: в `parent` обязательно есть `[[Linear algebra (field)]]`.
- Второй `parent` добавлять только если он очевиден; не больше 2.
- Для самой MOC: `notes/math/algebra/linal/512.64  Linear algebra MOC.md` имеет одного «родителя сверху» (решение в Chunk 0).

### `connected`

- `#обс/linking` заменяем на 3–8 конкретных `[[...]]`.
- В первую очередь связываем внутри `linal/`, во вторую — с несколькими внешними базовыми узлами.

### Legacy `links:`

- В `linal/` legacy `links:` удаляем полностью.
- Ссылки переносим в `parent`/`connected`.
- Удаляем весь «gap zone» (строки вида `links:` между `---` и контентом).

### `anki` и MOC/umbrella

- `anki` ставим только в entity/concept заметках (`true` при наличии Anki-блока, иначе `false`).
- В MOC/umbrella заметках поле `anki` отсутствует.

### Переименования

- В рамках миграции структуры/ссылок не переименовываем файлы через CLI.
- Если решаемся на нейминг/опечатки — делаем отдельной фазой через Obsidian UI.

## Процесс ревью (чанки <= 20 файлов)

На каждый чанк:

1) Я готовлю список изменений по каждому файлу (предлагаемые `parent`/`connected`, что удаляем/добавляем, какие новые файлы создаём).
2) Ты ревьювишь и правишь решения.
3) Я применяю правки ровно к этому чанку.

## План работ (последовательно)

### Chunk 0 — Решения до начала правок (обязательно)

- `notes/_meta/moc/512.64  Linear algebra MOC.md`: какой parent «сверху»?
  - оставить `[[512 Algebra]]` (как сейчас)
  - или сменить на `[[512.1 Elementary Algebra MOC]]` (чище по цепочке)
- `notes/math/algebra/linal/Linearity.md` (0 байт): что это?
  - линейность отображения (связать с `Linear Transformation`)
  - линейность функционала/оператора (может быть не linal)
- Anki: мигрируем ли `TARGET DECK: math::linal` → `stem::math::linal`?
  - да (отдельным чанком, строго сохраняя `ID`)
  - нет (фиксируем, что старые колоды остаются)

### Chunk 1 — Санитарный проход (схема + legacy `links:` + сломанный YAML + артефакты)

Цель: убрать явные технические проблемы, чтобы дальше работать спокойно.

Файлы (первый проход, 16 шт.):

- `notes/math/algebra/linal/512.64  Linear algebra MOC.md` (заменить `\(...\)` → `$...$`)
- `notes/_meta/moc/512.64  Linear algebra MOC.md` (заменить `\(...\)` → `$...$`)
- `notes/math/algebra/linal/Magic square.md` (удалить хвостовой мусор `04.png|150]]`)
- `notes/math/algebra/linal/Matrix.md` (добавить нормальный frontmatter)
- `notes/math/algebra/linal/Matrix Operations.md` (убедиться, что это umbrella; `anki` не ставить)
- `notes/math/algebra/linal/Basis VS.md` (добавить нормальный frontmatter, без сплитов пока)
- `notes/math/algebra/linal/Singular matrix.md` (добавить `parent/connected/tags/anki`)
- `notes/math/algebra/linal/Commutative matrix.md` (добавить `parent/created/tags`)
- `notes/math/algebra/linal/Augmented Matrices.md` (добавить `created/connected/tags/anki`)
- `notes/math/algebra/linal/Матрица линейного преобразования.md` (добавить `parent/connected/tags`; убрать конфликтный алиас)
- `notes/math/algebra/linal/Матрица перехода.md` (нормализовать `connected`, решить судьбу `fix/empty`)
- `notes/math/algebra/linal/Вращение (линейное преобразовние).md` (удалить legacy `links:`)
- `notes/math/algebra/linal/Растяжение-сжатие (линейное преобразовние).md` (починить `---` `---`, удалить legacy `links:`)
- `notes/math/algebra/linal/Переход из плоскости в пространство и обратно.md` (удалить legacy `links:`)
- `notes/math/algebra/linal/Сдвиг (линейное преобразовние).md` (подготовить к замене `#обс/linking`)
- `notes/math/algebra/linal/Hyperplane.md` (минимальный frontmatter/parent; пока без заполнения)
- `notes/math/algebra/linal/Linearity.md` (создать frontmatter-заготовку по решению из Chunk 0)

Особое:

- Конфликт терминов: `Матрица линейного преобразования.md` не должна иметь алиас `Матрица перехода`, т.к. есть отдельная заметка `Матрица перехода.md`.

### Chunk 2 — Убрать `#обс/linking` и проставить реальные `connected`

Цель: убрать плейсхолдеры и замкнуть граф linal.

Текущий список файлов с `#обс/linking` (14 шт., фактический набор после Chunk 1 может уменьшиться):

- `notes/math/algebra/linal/Calculation of the Matrix Determinant.md`
- `notes/math/algebra/linal/Determinant of matrix.md`
- `notes/math/algebra/linal/Eigen Values.md`
- `notes/math/algebra/linal/Elementary transformations.md`
- `notes/math/algebra/linal/Hyperplane.md`
- `notes/math/algebra/linal/Matrix Addition.md`
- `notes/math/algebra/linal/Matrix Vector Multiplication.md`
- `notes/math/algebra/linal/Span.md`
- `notes/math/algebra/linal/Trace of matrix.md`
- `notes/math/algebra/linal/Вращение (линейное преобразовние).md`
- `notes/math/algebra/linal/Линейная зависимость векторов.md`
- `notes/math/algebra/linal/Матрица перехода.md`
- `notes/math/algebra/linal/Переход из плоскости в пространство и обратно.md`
- `notes/math/algebra/linal/Сдвиг (линейное преобразовние).md`

### Chunk 3 — Закрыть `fix/empty` (довести до Level 1 без перфекционизма)

Цель: минимально заполнить реально пустые заметки и снять `fix/empty` там, где уже есть нормальный материал.

Кандидаты на заполнение (минимум: определение + 3–5 ссылок):

- `notes/math/algebra/linal/Euclidean space.md`
- `notes/math/algebra/linal/Zero vector.md`
- `notes/math/algebra/linal/Hyperplane.md`
- `notes/math/algebra/linal/Linearity.md`
- `notes/math/algebra/linal/Растяжение-сжатие (линейное преобразовние).md`

### Chunk 4 — Точность/смысл (минимальные правки утверждений)

Цель: убрать явные ошибки/смешение терминов.

Файлы-кандидаты (с ревью конкретных формулировок):

- `notes/math/algebra/linal/Determinant of matrix.md`
- `notes/math/algebra/linal/Trace of matrix.md`
- `notes/math/algebra/linal/Eigen Values.md`

### Chunk 5 — Anki-нормализация (без ломания `ID`)

Цель: привести карточки к текущим правилам `AGENTS-anki.md`.

Что уже найдено:

- Legacy тип карточки `Math_TWO_side` в 7 заметках:
  - `notes/math/algebra/linal/Kroneker delta.md`
  - `notes/math/algebra/linal/Identity matrix.md`
  - `notes/math/algebra/linal/Радиус-вектор.md`
  - `notes/math/algebra/linal/Column vector.md`
  - `notes/math/algebra/linal/Antidiagonal of square matrix.md`
  - `notes/math/algebra/linal/Diagonal matrix.md`
  - `notes/math/algebra/linal/Row vector.md`

Инварианты:

- `ID` никогда не удаляем и не пересоздаём.
- Конверсия `Math_TWO_side` → `math_basic_double`.

Доп. решение (из Chunk 0): что делать с `TARGET DECK: math::linal`.

### Chunk 6 — Разбить “толстые/перемешанные” заметки (single responsibility)

Цель: убрать мешанину и сделать заметки атомарными.

Кандидаты:

- `notes/math/algebra/linal/Basis VS.md`:
  - вынести темы в отдельные заметки (минимум): `Coordinates in a basis`, `Change of basis` (связать с `Матрица перехода`)
  - опционально: `Gram matrix`, `Orthonormal basis`, `Gram-Schmidt process`
- `notes/math/algebra/linal/Matrix.md`:
  - оставить определение матрицы
  - “равенство/эквивалентность” вынести в отдельные концепты (или привести к норме существующие `Matrix Comparasion.md` и т.п.)
  - свойства операций распределить по `Matrix Operations.md` и атомарным операциям
- `notes/math/algebra/linal/Calculation Matrix Inverse.md`:
  - если внутри смешаны разные темы (adjugate/row ops vs image/preimage) — разнести
- `notes/math/algebra/linal/Линейная зависимость векторов.md`:
  - отделить atomic definition от набора критериев/геометрических следствий
- `notes/math/algebra/linal/512.64  Linear algebra MOC.md`:
- `notes/_meta/moc/512.64  Linear algebra MOC.md`:
  - оставить как индекс
  - рассуждения/таблицы вынести в отдельные концепты и линковать из MOC

### Chunk 7 — (опционально) Нейминг/опечатки (только через Obsidian UI)

Кандидаты:

- `Kroneker delta.md` → `Kronecker delta.md`
- `Row-Echelone form REF.md` → `Row-echelon form (REF).md`
- `Reduced Row-Echelon form RREF.md` → `Reduced row-echelon form (RREF).md`
- `Matrix Comparasion.md` → `Matrix equality.md` (или иное название)
- `Eigen Values.md` → `Eigenvalues.md`
- Русские файлы с опечаткой “преобразовние” → нормализовать
