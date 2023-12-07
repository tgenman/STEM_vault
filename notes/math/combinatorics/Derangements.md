---
aliases:
  - Перестановки без неподвижных точек
publish: true
anki: true
created: 2023-10-30 20:35
parent:
  - "[[Arrangements without repetition]]"
connected: []
---

$$d_n=n!\left(1-\frac{1}{1!}+\frac{1}{2!}-\ldots+(-1)^n\frac{1}{n!}\right)$$

$$
d_n\sim\frac{n!}e
$$


#### Proof
$d_n = |U| - \sum_i |A_i| + \sum_{i,j} |A_i \cap A_j| + \ldots$  
If $S \subset \{1, \ldots, n\}$ let $M = \cap_{j \in S} A_j$.  
$M$ is the set of permutations $\pi$ with $\pi(j) = j$ for all $j \in S$. Then $|M| = A_{n-|S|} = (n-|S|)!$.  

Hence, $\sum_{S \subset \{1, \ldots, n\}, |S| = k} |\cap_{j \in S} A_j| = \binom{n}{k} \cdot (n-k)! = \frac{n!}{(n-k)!k!} (n-k)! = \frac{n!}{k!}$.

$d_n = |U| - \sum_i |A_i| + \sum_{i,j} |A_i \cap A_j| + \ldots = n! - \frac{n!}{1!} + \frac{n!}{2!} - \ldots + (-1)^n \frac{n!}{n!} = n!\left(1 - \frac{1}{1!} + \frac{1}{2!} - \ldots + (-1)^n \frac{1}{n!}\right)$.


### Anki
TARGET DECK: Math::Combinatorics  
START
Math prop
Question_eng: Derangements
Question_rus: Перестановки без неподвижных точек
Answer_eng: $$d_n=n!\left(1-\frac{1}{1!}+\frac{1}{2!}-\ldots+(-1)^n\frac{1}{n!}\right)$$
Answer_rus: 
Formula_main: Proof
$d_n = |U| - \sum_i |A_i| + \sum_{i,j} |A_i \cap A_j| + \ldots$  
If $S \subset \{1, \ldots, n\}$ let $M = \cap_{j \in S} A_j$.  
$M$ is the set of permutations $\pi$ with $\pi(j) = j$ for all $j \in S$. Then $|M| = A_{n-|S|} = (n-|S|)!$.  

Hence, $\sum_{S \subset \{1, \ldots, n\}, |S| = k} |\cap_{j \in S} A_j| = \binom{n}{k} \cdot (n-k)! = \frac{n!}{(n-k)!k!} (n-k)! = \frac{n!}{k!}$.

$d_n = |U| - \sum_i |A_i| + \sum_{i,j} |A_i \cap A_j| + \ldots = n! - \frac{n!}{1!} + \frac{n!}{2!} - \ldots + (-1)^n \frac{n!}{n!} = n!\left(1 - \frac{1}{1!} + \frac{1}{2!} - \ldots + (-1)^n \frac{1}{n!}\right)$.

Formula_additional:
<!--ID: 1698688139448-->
END

START
Math prop
Question_eng: Approximate value of Derangements
Question_rus: 
Answer_eng: $$d_n\sim\frac{n!}e$$
Answer_rus: 
Formula_main: 
Formula_additional:
<!--ID: 1698688139452-->
END




