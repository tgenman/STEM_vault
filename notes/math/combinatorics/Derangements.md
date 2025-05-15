---
aliases:
  - Перестановки без неподвижных точек
  - Субфакториал
  - Смещения
  - Беспорядки
anki: false
created: 2023-10-30 20:35
parent:
  - "[[Permutatios without repetitions]]"
  - "[[Factorial]]"
connected:
---

> [!tip] Derangements, смещения
число перестано­вок $n$ элементов, при кото­рых ни один из элементов не стоит на своем месте
$$D_n=n!\left(1-\frac{1}{1!}+\frac{1}{2!}-\ldots+(-1)^n\frac{1}{n!}\right) = !n$$

$D_n = P_n - \binom{n}{1} P_{n-1} + \binom{n}{2} P_{n-2} - \ldots + (-1)^n \binom{n}{n} = n! \left[ 1 - \frac{1}{1!} + \frac{1}{2!} - \ldots + \frac{(-1)^n}{n!} \right].$

Число перестановок, при которых ровно $r$ элементов остаются на первоначальных местах, а остальные $n - r$ меняют свое положение, выражается формулой $$D_{n,r} = C_n^r D_{n-r}.$$
Разобьем все перестановки на классы в зависимости от того, сколько элементов остаются неподвижными при данной перестановке. Так как общее число перестановок равно $n!$, то получаем следующее тождество: $$n! = \sum_{r=0}^{n} D_{n,r} = \sum_{r=0}^{n} C_n^r D_{n-r}.$$
#### Субфакториалы (похожи на [[Factorial]])
Покажем, что это же равенство верно и для субфакториалов $D_n$. Т. е., что $$D_n = (n - 1)(D_{n-1} + D_{n-2}).$$





#### Approximate value of Derangements
$$
d_n\sim\frac{n!}e
$$

#### Properties



#### Proof
$d_n = |U| - \sum_i |A_i| + \sum_{i,j} |A_i \cap A_j| + \ldots$  
If $S \subset \{1, \ldots, n\}$ let $M = \cap_{j \in S} A_j$.  
$M$ is the set of permutations $\pi$ with $\pi(j) = j$ for all $j \in S$. Then $|M| = A_{n-|S|} = (n-|S|)!$.  

Hence, $\sum_{S \subset \{1, \ldots, n\}, |S| = k} |\cap_{j \in S} A_j| = \binom{n}{k} \cdot (n-k)! = \frac{n!}{(n-k)!k!} (n-k)! = \frac{n!}{k!}$.

$d_n = |U| - \sum_i |A_i| + \sum_{i,j} |A_i \cap A_j| + \ldots = n! - \frac{n!}{1!} + \frac{n!}{2!} - \ldots + (-1)^n \frac{n!}{n!} = n!\left(1 - \frac{1}{1!} + \frac{1}{2!} - \ldots + (-1)^n \frac{1}{n!}\right)$.


# Anki
TARGET DECK: math::combinatorics  
START
Math_ONE_side
TITLE: Derangements
Перестановки без неподвижных точек, Смещения
DESCRIPTION: число перестано­вок $n$ элементов, при кото­рых ни один из элементов не стоит на своем месте
$$d_n=n!\left(1-\frac{1}{1!}+\frac{1}{2!}-\ldots+(-1)^n\frac{1}{n!}\right)$$
FORMULA: $D_n = P_n - \binom{n}{1} P_{n-1} + \binom{n}{2} P_{n-2} - \ldots + (-1)^n \binom{n}{n} = n! \left[ 1 - \frac{1}{1!} + \frac{1}{2!} - \ldots + \frac{(-1)^n}{n!} \right].$
ADDITIONAL:
ID: 1698688139448
END

TARGET DECK: math::combinatorics  
START
Math_ONE_side
TITLE: Approximate value of Derangements
DESCRIPTION: $$d_n\sim\frac{n!}e$$
FORMULA: 
ADDITIONAL:
ID: 1698688139452
END




