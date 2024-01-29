---
aliases: 
tags:
  - theorem
publish: true
anki: true
created: 2023-10-21 17:58
parent:
  - "[[Equivalence Relation]]"
  - "[[Partition of a set]]"
connected:
---

Let $S$ be a  nonempty set and let $∼$ be an [[Equivalence Relation]]  on $S$. Then $∼$ yields a  [[Partition of a set]] of $S$, where

$$
\bar{a}=\{x\in S\mid x\sim a\}.
$$

Also, each partition of $S$ gives rise to an equivalence relation $∼$ on $S$ where $a ∼ b$ if and only if a and b are in the same cell of the partition.

### Proof
We must show that the different cells $\bar{a} = \{ x\in S|x\sim a\}$ for $a\in S$ do give a partition of $S$, so that every element of $S$ is in some cell and so that if $\alpha\in \bar{b}$ , then $\bar{a} = \bar{b}$. Let $a\in S.$ Then $a\in\bar{a}$ by the reflexive condition (1), so $a$ is in at least one cell.

Suppose now that $a\in\bar{b}.$ We need to show that $\bar{a}=\bar{b}$ as sets; this will show that $a$ cannot be in more than one cell. There is a standard way to show that two sets are the same:

Show that each set is $a$ subset of the other.

We show that $\bar{a}\subseteq\bar{b}$. Let $x\in\bar{a}.$ Then $x\sim a.$But$a\in \bar{b} , $so$a\sim b.$ Then, by the transitive condition $( 3) , x\sim b, $so $x\in \bar{b} .$ Thus $\bar{a}\subseteq\bar{b}.$ Now we show that $\bar{b}\subseteq\bar{a}.$ Let $y\in\bar{b}.$ Then $y\sim b$. But $a\in \bar{b} , $so$a\sim b$ and, by symmetry $(2),b\sim a.$ Then by transitivity (3), $y\sim a$, so $y\in\bar{a}$. Hence $\bar{b}\subseteq\bar{a}$ also, so $\bar{b}=\bar{a}$ and our proof is complete.

### Anki
TARGET DECK: Math::Set  
START
Math prop
TITLE: Equivalence Relations and Partitions (theorem)
TITLE_rus: 
Answer_eng: Let $S$ be a  nonempty set and let $∼$ be an [[Equivalence Relation]]  on $S$. Then $∼$ yields a  [[Partition of a set]] of $S$, where

$$
\bar{a}=\{x\in S\mid x\sim a\}.
$$

Also, each partition of $S$ gives rise to an equivalence relation $∼$ on $S$ where $a ∼ b$ if and only if a and b are in the same cell of the partition.
Answer_rus: 
Formula_main: 
Formula_additional:
<!--ID: 1697900657287-->
END









