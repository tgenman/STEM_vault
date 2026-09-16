---
aliases:
  - Система линейных уравнений (СЛУ)
parent:
  - "[[Linear algebra (field)]]"
---

### Solution Set 
- A _solution_ of a system of equations is a list of numbers x,y,z,... that make all of the equations true simultaneously.
- The _solution set_ of a system of equations is the collection of all solutions.
- _Solving_ the system means finding all solutions with formulas involving some number of parameters.
A system of equations is called _inconsistent_ if it has no solutions. It is called _consistent_ otherwise.



### Solution Methods

- Решение через нахождение [[Matrix Inverse]] — если $A$ квадратная и обратимая
$$A⋅X=B$$
$$A^{−1}A⋅X=A^{−1}B⇔EX=A^{−1}B⇔X=A^{−1}B$$

- [[The Gaussian Elimination Method]]

## однородная система

A linear system $Ax=b$ is homogeneous when $b=0$. It is always consistent because $x=0$ is a solution. Nonzero solutions may also exist; see [[Линейная зависимость векторов]] and [[Matrix Inverse#обратимость и нулевое решение]].

Источник переноса: [[512.64  Linear algebra MOC]].
