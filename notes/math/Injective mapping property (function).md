---
aliases:
  - One-to-one function mapping
publish: true
anki: false
created: 2023-10-17 21:13
parent: 
connected:
  - "[[Bijective mapping property]]"
tags:
---


A special type of relation $↔$ between $X$ and $Y$ called a ==one-to-one correspondence==. Since each element $x$ of $X$ appears precisely once in this relation, we can regard this one-to-one correspondence as a function with [[Domain Dom(f) or Preimage]] $X$. 

The [[Range Ran(f) or Image Im(f)]]  is $Y$ because each $y$ in $Y$ also appears in some pairing $x ↔ y$.


Инъективное . У одного  образа не больше одного праобраза #анки 

Injective property

We can think of $injective$ functions as pipes that transport fluids between containers. Since fluids cannot be compressed, the "output container" must be at least as large as the "input container." If there are two distinct points $x_1$ and $x_2$ in the input container of an injective function, then there will be two distinct points $f(x_1)$ and $f(x_2)$ in the output container of the function as well. In other words, injective functions don’t smoosh things together.

In contrast, a function that doesn’t have the injective property can map several different inputs to the same output value. The function $f(x) = x^2$ is not injective since it sends inputs $x$ and $-x$ to the same output value $f(x) = f(-x) = x^2$, as illustrated in Figure 1.16.

The maps-distinct-inputs-to-distinct-outputs property of injective functions has an important consequence: given the output of an injective function $y$, there is only one input $x$ such that $f(x) = y$. If a second input $x'$ existed that also leads to the same output $f(x) = f(x') = y$, then the function $f$ wouldn’t be injective. For each of the outputs $y$ of an injective function $f$, there is a $unique$ input $x$ such that $f(x) = y$. In other words, injective functions have a $unique$-$input$-$for$-$each$-$output$ property.




![[Pasted image 20230915113741.png]]



