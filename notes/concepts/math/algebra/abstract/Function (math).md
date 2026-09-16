---
aliases:
  - Функция
  - Single-valued mapping
  - Отображение
anki: false
created: 2023-09-15 11:18
parent:
  - "[[Mapping (math)]]"
  - "[[Operations on sets]]"
connected:
  - "[[517 Сalculus MOC|Calculus]]"
  - "[[512.1 Elementary Algebra MOC]]"
  - "[[Inverse function (math)]]"
  - "[[Function composition]]"
---


> [!tip] Функция
это [[Mapping (math)|отображение]]  одного [[Set (math)|множества]]  в другое, где каждому элементу первого множества соответствует только один элемент второго.

> [!tip] A function $φ$
 mapping $X$ into $Y$ is a [[Mapping (math)]] between $X$ and $Y$ with the property that each $x ∈ X$ appears as the first member of exactly one ordered pair $(x, y)$ in $φ$. 

Such a function is also ca[](Relation.md)=mapping== of $X$ into $Y$. 
We write $φ : X → Y$ and express $(x, y) ∈ φ$ by $φ(x) = y$ 
$$f:X⟶Y$$
- The [[Domain Dom(f) or Preimage|domain]] of $φ$ is the set $X$ and 
- The set $Y$ is the[[Codomain of a function|codomain]] of $φ$.  
- The [[Range Ran(f) or Image Im(f)|range]] of $φ$ is $φ[X] = \set{φ(x) | x ∈ X}$. 

![[Pasted image 20240117200108.png|300]]
![[Pasted image 20240117205354.png|300]]


Illustration of the input and output sets of a function $f : A -> B$. The ==source set== is denoted $A$ and the domain is denoted $Dom(f)$. Note that the function’s [[Domain Dom(f) or Preimage|domain]]  is a subset of its ==source set==. The target set is denoted $B$ and the image is denoted $Imp(f)$. 
The [[Range Ran(f) or Image Im(f)|Image of a function]] is a subset of the ==target set==.

Примеры отображения числовых множеств:
$f:R⟶R,$
$g:N⟶R∖{3},$
$p:Z⟶[1; 7],$
$q:(3; 4)⟶{0; 1}.$

Множества в отображении необязательно должны быть числовыми. Их элементами могут быть векторы, матрицы, функции, другие множества. Вот, например, множество из трёх векторов отображается во множество из двух чисел: ${(2, 3), (0, 4), (5, 7)}⟶{2, 1}$.

## исходные фрагменты из карты общей алгебры

Источник переноса: [[512.5 General Algebra MOC]]. Содержательная проверка не выполнялась.

**Функция** – это общее математическое понятие, описывающее соответствие между двумя множествами, где каждому элементу из одного множества ставится в соответствие единственный элемент из другого множества.

**Формальное определение:**
Функция $f: \mathcal{A} \to \mathcal{B}$ – это правило, которое каждому элементу $x \in \mathcal{A}$ ставит в соответствие единственный элемент $f(x) \in \mathcal{B}$.

**Примеры:**
- Функция $f(x) = x^2$, где $\mathcal{A} = \mathbb{R}$ и $\mathcal{B} = \mathbb{R}$.
- Функция $g(x) = \sin(x)$, где $\mathcal{A} = \mathbb{R}$ и $\mathcal{B} = [-1, 1]$.

- **Функция**: Пусть $\mathcal{A} = \mathbb{R}$ и $\mathcal{B} = \mathbb{R}$. Функция $f: \mathcal{A} \to \mathcal{B}$ определяется как $f(x) = x^2$. Здесь $\mathcal{A}$ и $\mathcal{B}$ могут быть разными множествами.

1. **Простая функция:**
   Пусть $\mathcal{A} = \{1, 2, 3\}$ и $\mathcal{Б} = \{a, b, c\}$. Отображение $f: \mathcal{A} \to \mathcal{Б}$ может быть задано правилом: $f(1) = a$, $f(2) = b$, $f(3) = c$.

2. **Арифметическая функция:**
   Пусть $\mathcal{A} = \mathbb{R}$ и $\mathcal{Б} = \mathbb{R}$. Отображение $f: \mathcal{A} \to \mathcal{Б}$ задано формулой $f(x) = x^2$. Здесь каждому вещественному числу $x$ соответствует его квадрат $x^2$.

1. **Простая функция:**
   Пусть $\mathcal{A} = \{1, 2, 3\}$ и $\mathcal{Б} = \{a, b, c\}$. Функция $f: \mathcal{A} \to \mathcal{Б}$ может быть задана правилом: $f(1) = a$, $f(2) = b$, $f(3) = c$.

2. **Арифметическая функция:**
   Пусть $\mathcal{A} = \mathbb{R}$ и $\mathcal{Б} = \mathmathbb{R}$. Функция $f: \mathcal{A} \to \mathcal{Б}$ задана формулой $f(x) = x^2$. Здесь каждому вещественному числу $x$ соответствует его квадрат $x^2$.

Функции могут обладать различными свойствами, такими как инъективность, сюръективность и биективность:
