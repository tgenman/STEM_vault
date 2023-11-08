---
aliases:
  - Формула включений-исключений
publish: true
anki: false
created: 2023-10-20 21:01
parent:
  - "[[510.22 Sets theory MOC]]"
connected:
  - "[[519.21  Probability theory|Probability theory]]"
  - "[[Cardinality]]"
tags:
  - empty
---
$$
\begin{aligned}P(A_1 \cup ... \cup A_k)=&P(A_1)+...+P(A_n)-P(A_1\cap A_2)-P(A_1\cap A_3)-...-\\&-P(A_{k-1}\cap A_k)+...+(-1)^{k-1}P(A_1\cap ... \cap A_k).\end{aligned}
$$

### Для трёх множеств
$$\begin{aligned}
|A\cup B\cup C|=& |A|+|B|+|C|-  \\
&-|A\cap B|-|A\cap C|-|B\cap C|+ \\
&+|A\cap B\cap C|
\end{aligned}$$

![[Pasted image 20231020210108.png|300]]

Given an integer N. You have to print a sequence of numbers from 11 to NN. But print "Fizz" if the number is a multiple of 3, "Buzz" if the number is a multiple of 55 and "Fizz Buzz" if the number is a multiple of 1515.
