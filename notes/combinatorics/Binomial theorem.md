---
aliases:
  - Биномиальная теорема
  - Бином Ньютона
publish: true
anki: true
created: 2023-10-23 18:17
parent:
  - "[[519.101 Combinatorics]]"
  - "[[Pascal’s triangle]]"
connected:
  - "[[Binomial coefficient]]"
  - "[[517.52 Ряды и последовательности]]"
  - "[[Неравенство Бернулли]]"
tags:
  - theorem
---
$$(a + b)^n = \sum\limits_{k=0}^n \binom{n}{k} a^{n-k} b^k = $$
$$=\binom n0a^n+\binom n1a^{n-1}b+\ldots+\binom nnb^n$$

### Proof
$$\begin{aligned}
&\textsf{Binomial Theorem. Proof} \\
&\begin{array}{l}(a+b)^n=\sum_{k=0}^n\binom nka^{n-k}b^k.\\\rhd(a+b)^n=(a+b)\cdotp(a+b)\cdotp...\cdotp(a+b)\end{array} \\
&a^kb^{n-k}:\quad\mathrm{choose~a~exactly~k~times} \\
&\text{from brackets.} \\
&\text{Hence, the coefficient is equal to} \\
&\begin{pmatrix}n\\k\end{pmatrix}.
\end{aligned}$$
$$\begin{aligned}
&\text{Binomial Theorem. Proof 2} \\
&\rhd\text{ By induction. }\quad\mathrm{Base:}\quad\mathrm{(a~+~b)~=} \\
&\binom11\text{а }+\mathrm{~}\binom10\text{b. Suppose that identity} \\
&\begin{array}{rcl}(a_1+b)^n&=&(a_1+b)^{n-1}(a_1+b)&=\\\sum_{k=0}^{n-1}\binom{n-1}ka^{n-1-k}b^k(a_1+b)&=\end{array} \\
&\text{一个} \\
&\sum_{k=0}^{n-1}\binom{n-1}k(a^{n-k}b^k+a^{n-1-k}b^{k+1})= \\
&\sum_{k=0}^na^{n-k}b^k(\binom{n-1}k+\binom{n-1}{k+1})= \\
&\sum_{k=0}^n\binom nka^{n-k}b^k.\quad\square 
\end{aligned}$$

### Anki
TARGET DECK: Math::Combinatorics
START
Math prop
Question_eng: Binomial theorem
Question_rus: 
Answer_eng: $$(a + b)^n = \sum\limits_{k=0}^n \binom{n}{k} a^{n-k} b^k = $$
$$=\binom n0a^n+\binom n1a^{n-1}b+\ldots+\binom nnb^n$$
Answer_rus: 
Formula_main: $$\begin{aligned}
&\textsf{Binomial Theorem. Proof} \\
&\begin{array}{l}(a+b)^n=\sum_{k=0}^n\binom nka^{n-k}b^k.\\\rhd(a+b)^n=(a+b)\cdotp(a+b)\cdotp...\cdotp(a+b)\end{array} \\
&a^kb^{n-k}:\quad\mathrm{choose~a~exactly~k~times} \\
&\text{from brackets.} \\
&\text{Hence, the coefficient is equal to} \\
&\begin{pmatrix}n\\k\end{pmatrix}.
\end{aligned}$$
$$\begin{aligned}
&\text{Binomial Theorem. Proof 2} \\
&\rhd\text{ By induction. }\quad\mathrm{Base:}\quad\mathrm{(a~+~b)~=} \\
&\binom11\text{а }+\mathrm{~}\binom10\text{b. Suppose that identity} \\
&\begin{array}{rcl}(a_1+b)^n&=&(a_1+b)^{n-1}(a_1+b)&=\\\sum_{k=0}^{n-1}\binom{n-1}ka^{n-1-k}b^k(a_1+b)&=\end{array} \\
&\text{一个} \\
&\sum_{k=0}^{n-1}\binom{n-1}k(a^{n-k}b^k+a^{n-1-k}b^{k+1})= \\
&\sum_{k=0}^na^{n-k}b^k(\binom{n-1}k+\binom{n-1}{k+1})= \\
&\sum_{k=0}^n\binom nka^{n-k}b^k.\quad\square 
\end{aligned}$$

Formula_additional:
<!--ID: 1698689820218-->
END










