---
aliases:
  - Биномиальная теорема
  - Бином Ньютона
anki: true
created: 2023-10-23 18:17
parent:
  - "[[Pascal’s triangle]]"
  - "[[Multinomial formula]]"
connected:
  - "[[Binomial theorem]]"
  - "[[519.101 Combinatorics MOC]]"
tags:
  - theorem
---

$$(a + b)^n = \sum\limits_{k=0}^n \binom{n}{k} a^{n-k} b^k = $$
$$=\binom n0a^n+\binom n1a^{n-1}b+\ldots+\binom nnb^n$$

### Proof
Binomial Theorem. Proof

$$(a+b)^n=\sum_{k=0}^n\binom{n}{k}a^{n-k}b^k. \rhd (a+b)^n=(a+b)\cdotp(a+b)\cdotp...\cdotp(a+b)$$

To obtain $a^k b^{n-k}$: choose 'a' exactly k times from the brackets. Hence, the coefficient is equal to $\binom{n}{k}$.

Binomial Theorem. Proof 2

$$\rhd\text{By induction.}\quad\mathrm{Base:}\quad\mathrm{(a~+~b)~=} \binom{1}{1}a + \binom{1}{0}b. \text{Suppose that identity}$$

$$(a_1+b)^n=(a_1+b)^{n-1}(a_1+b)=\sum_{k=0}^{n-1}\binom{n-1}{k}a^{n-1-k}b^k(a_1+b)$$

$$=\sum_{k=0}^{n-1}\binom{n-1}{k}(a^{n-k}b^k+a^{n-1-k}b^{k+1})=\sum_{k=0}^na^{n-k}b^k\left(\binom{n-1}{k}+\binom{n-1}{k+1}\right)=\sum_{k=0}^n\binom{n}{k}a^{n-k}b^k. \quad\square$$


### Anki
> [!question]-
TARGET DECK: Math::Combinatorics
START
Math_ONE_side
TITLE: Binomial theorem
DESCRIPTION: $$(a + b)^n = \sum\limits_{k=0}^n \binom{n}{k} a^{n-k} b^k = $$
$$=\binom n0a^n+\binom n1a^{n-1}b+\ldots+\binom nnb^n$$
FORMULA: Binomial Theorem. Proof

$$(a+b)^n=\sum_{k=0}^n\binom{n}{k}a^{n-k}b^k. \rhd (a+b)^n=(a+b)\cdotp(a+b)\cdotp...\cdotp(a+b)$$

To obtain $a^k b^{n-k}$: choose 'a' exactly k times from the brackets. Hence, the coefficient is equal to $\binom{n}{k}$.

Binomial Theorem. Proof 2

$$\rhd\text{By induction.}\quad\mathrm{Base:}\quad\mathrm{(a~+~b)~=} \binom{1}{1}a + \binom{1}{0}b. \text{Suppose that identity}$$

$$(a_1+b)^n=(a_1+b)^{n-1}(a_1+b)=\sum_{k=0}^{n-1}\binom{n-1}{k}a^{n-1-k}b^k(a_1+b)$$

$$=\sum_{k=0}^{n-1}\binom{n-1}{k}(a^{n-k}b^k+a^{n-1-k}b^{k+1})=\sum_{k=0}^na^{n-k}b^k\left(\binom{n-1}{k}+\binom{n-1}{k+1}\right)=\sum_{k=0}^n\binom{n}{k}a^{n-k}b^k. \quad\square$$

ADDITIONAL:
ID: 1698689820218
END










