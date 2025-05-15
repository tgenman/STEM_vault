---
aliases:
  - Скалярное произведение в евклидовом пространстве
anki: true
created: 2024-02-03 18:17
parent:
  - "[[Inner product of vectors]]"
connected:
  - "[[Euclidian norm (L2)]]"
---

> [!tip] Dot product 
это частный случай [[Inner product of vectors]]
$\vec{a} \cdot \vec{b} = a_x b_x + a_y b_y + a_z b_z = (\vec{a}, \vec{b})$ 
$\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos{\phi}$
Commonly, the dot product between two vectors $a, b$ is denoted by $a^\top b$ or $\langle a, b \rangle$.


$\cos(\vec{a},\vec{b})=\frac{\vec{a}\cdot\vec{b}}{|\vec{a}|\cdot|\vec{b}|}$

$\cos(\vec{a},\vec{b})=\frac{a_1\cdot b_1+a_2\cdot b_2}{\sqrt{{a_1}^2+{a_2}^2}\cdot\sqrt{{b_1}^2+{b_2}^2}}.$


![[Pasted image 20220719125413.png|500]]


#### Properties
- [[Commutative identity]] 
    $\vec{b} \cdot \vec{a} = \vec{a} \cdot \vec{b}$
-  [[Associative identity|ассоциативность]]  произведения
    $(k \cdot \vec{a}) \cdot \vec{b} = k \cdot (\vec{a} \cdot \vec{b})$
- [[Distributive|дистрибутивность]] [[Scalar|скалярного]] произведения
    $(\vec{a} + \vec{b}) \cdot \vec{c} = \vec{a} \cdot \vec{c} + \vec{b} \cdot \vec{c}$


# Anki
TARGET DECK: math::linal 
START
Math_ONE_side
TITLE: Dot product of vectors
DESCRIPTION: это частный случай [[Inner product of vectors]]
FORMULA: $\vec{a} \cdot \vec{b} = a_x b_x + a_y b_y + a_z b_z = (\vec{a}, \vec{b})$ 
$\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos{\phi}$
Commonly, the dot product between two vectors $a, b$ is denoted by $a^\top b$ or $\langle a, b \rangle$.
ADDITIONAL:
PICTURE: ![[Pasted image 20220719125413.png|500]]
ID: 1707598158528
END


TARGET DECK: math::linal 
START
Math_ONE_side
TITLE: Properties of Dot product of vectors
DESCRIPTION: 
- [[Commutative identity]] $\vec{b} \cdot \vec{a} = \vec{a} \cdot \vec{b}$
- [[Associative identity|ассоциативность]]  произведения $(k \cdot \vec{a}) \cdot \vec{b} = k \cdot (\vec{a} \cdot \vec{b})$
- [[Distributive|дистрибутивность]] [[Scalar|скалярного]] произведения $(\vec{a} + \vec{b}) \cdot \vec{c} = \vec{a} \cdot \vec{c} + \vec{b} \cdot \vec{c}$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1707598158544
END