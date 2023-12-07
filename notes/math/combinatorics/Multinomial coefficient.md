---
aliases: 
publish: true
anki: false
created: 2023-11-11 13:27
parent:
  - "[[Permutations with repetitions]]"
connected:
  - "[[Binomial coefficient]]"
---
The multinomial coefficient is a generalization of the [[Binomial coefficient]].

> [!tip] Multinomial coefficient
> по сути это просто [[Permutatios without repetitions]] with repetitions

> [!tip] Multinomial coefficient
For a given non-negative integer ${} n {}$ and a given [[Tuple]] tuple of non-negative integers ${} (k_1,k_2,…,k_m) {}$ such that the sum of all ${} k_i {}$​ is $n {}$ (i.e., ${} k_1+k_2+…+k_m=n {}$),  calculated as:
$${} P(k_1, k_2, ..., k_m) =  \binom{n}{k_1,k_2,…,k_m}=\frac{n!}{k_1!⋅k_2!⋅…⋅k_m!}​=M(n_1,...,n_k) {}$$

#### Examples in Combinatorics:

1. **Dividing a Group into Smaller Groups**:
   - **Problem**: In how many ways can 10 students be divided into three study groups containing 4, 3, and 3 students, respectively?
   - **Solution**: This can be solved using the multinomial coefficient: 
$\binom{10}{4, 3, 3} = \frac{10!}{4! \cdot 3! \cdot 3!}$

2. **Distributing Objects into Boxes**:
   - **Problem**: Imagine you have 6 different fruits and want to distribute them into 3 different baskets, with 2 fruits in each basket.
   - **Solution**: The number of ways to do this distribution is given by the multinomial coefficient  $\binom{6}{2, 2, 2}$ , which equals  $\frac{6!}{2! \cdot 2! \cdot 2!}$.


#### Proof

$$
\binom n{n_1,n_2,...,n_k}=\frac{n!}{n_1!n_2!\cdot...\cdot n_k!}
$$
 Suppose $S$ have elements ${} x_1,\ldots,x_k$ with $n_1,\ldots,n_k$ repetitions resp. Permutation: place $x_{1}.$ We have ${\binom n{n_1}}$ ways to do this.

 Then we place $x_2.$ We have $\binom{n-n_1}{n_2}$  ways to do this.

The number of permutations of S equals:

$$
\begin{array}{c}
\binom{n}{n_1} \cdot \binom{n-n_1}{n_2} \cdot \binom{n-n_1-n_2}{n_3} \cdots \binom{n-n_1-\ldots-n_{k-1}}{n_k}
\end{array}
$$

$$
=\frac{n!}{n_1!(n-n_1)!} \cdot \frac{(n-n_1)!}{n_2!(n-n_1-n_2)!} \cdot \frac{(n-n_1-n_2)!}{n_3!(n-n_1-n_2-n_3)!} \cdots \frac{(n-n_1-\ldots-n_{k-1})!}{n_k!(n-n_1-\ldots-n_{k})!}
$$

$$
=\frac{n!}{n_1!n_2!\cdots n_k!}
$$



