---
aliases:
  - Скалярное произведение в евклидовом пространстве
publish: true
anki: false
created: 2024-02-03 18:17
parent:
  - "[[Inner product of vectors]]"
connected:
  - "[[Euclidian norm (L2)]]"
---

> [!tip] Dot product 
это частный случай [[Inner product of vectors]]
$\vec{a} \cdot \vec{b} = a_x b_x + a_y b_y + a_z b_z = (\vec{a}, \vec{b})$ 

$\vec{a} = a_x \vec{i} + a_y \vec{j} + a_z \vec{k}$  
$\vec{b} = b_x \vec{i} + b_y \vec{j} + b_z \vec{k}$ 
$\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos{\phi}$


$\cos(\vec{a},\vec{b})=\frac{\vec{a}\cdot\vec{b}}{|\vec{a}|\cdot|\vec{b}|}$

$\cos(\vec{a},\vec{b})=\frac{a_1\cdot b_1+a_2\cdot b_2}{\sqrt{{a_1}^2+{a_2}^2}\cdot\sqrt{{b_1}^2+{b_2}^2}}.$


![[Pasted image 20220719125413.png|500]]


Для скалярного произведения действуют несколько свойств. О свойстве коммутативности вы уже знаете. А вот ещё два:
- $(k \cdot \vec{a}) \cdot \vec{b} = k \cdot (\vec{a} \cdot \vec{b})$ — ассоциативность скалярного произведения: скаляр $k$ из него можно вынести за скобки.
- $(\vec{a} + \vec{b}) \cdot \vec{c} = \vec{a} \cdot \vec{c} + \vec{b} \cdot \vec{c}$ — дистрибутивность скалярного произведения.



