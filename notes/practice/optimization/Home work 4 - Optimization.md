author: **Dmitrii Bondarev** (Дмитрий Бондарев)
group: М05-321сс (**Contemporary Combinatorics**)
date: 2024-12-16

## 1. (2 pts) What claims from below list are correct and what are incorrect and why?

- ☐ Any convex function is smooth  
- ☐ Any strongly convex function has unique global minimum  
- ☐ If convex function is bounded below, then it has a unique point of minimum $\mathbf{x}^*$  
- ☐ A strongly convex function is always differentiable  

1. **"Any convex function is smooth"**: **No**  
    Convexity doesn't guarantee smoothness. Take $f(x) = |x|$ - it's convex but not differentiable at $x = 0$. Convexity only tells us about the function's shape, not its smoothness.

2. **"Any strongly convex function has a unique global minimum"**: **Yes**  
    Strongly convex functions must curve upward with some positive $m$, which prevents flat regions. This guarantees exactly one minimum point, like a strict bowl shape.

3. **"If a convex function is bounded below, then it has a unique point of minimum $x^*$"**: **No**  
    Counter-example: $f(x) = 0$ is convex and bounded below, but every point is a minimum. Being bounded below doesn't force a unique minimum.

4. **"A strongly convex function is always differentiable"**: **No**  
    Consider $f(x) = x^2 + |x|$. The $x^2$ part makes it strongly convex, but $|x|$ creates a non-differentiable point at $x = 0$. Strong convexity only ensures growth rate, not smoothness.

---


## 2. (7 pts) What functions below are convex or concave and why?
- ☐ $f(\mathbf{x}) = \sup_{\mathbf{y} \in C} \langle \mathbf{y}, \mathbf{x} \rangle$, where $C$ is some given set  
- ☐ $f(\mathbf{x}) = \|\mathbf{A}\mathbf{x} - \mathbf{b}\|$, where $\|\cdot\|$ is an arbitrary norm  
- ☐ $f(\mathbf{x}) = \min_{i=1, \dots, m} x_i$  
- ☐ $f(\mathbf{x}) = -\left(\prod_{i=1}^n x_i\right)^{1/n}$, dom $f = \mathbb{R}^n_+$  
- ☐ $f(\mathbf{w}) = \sum_{i=1}^m \log(1 + e^{-y_i \mathbf{w}^\top \mathbf{x}_i}) + \frac{1}{2}\|\mathbf{w}\|^2$, where $\mathbf{x}_i \in \mathbb{R}^n$, $y_i \in \mathbb{R}$. This function is basic loss for binary classification problem.  
- ☐ $f(\mathbf{X}, \mathbf{Y}) = \|\mathbf{A} - \mathbf{X}\mathbf{Y}\|_F^2$, where $\mathbf{X} \in \mathbb{R}^{m \times p}$, $\mathbf{Y} \in \mathbb{R}^{p \times n}$. The notation $\|\cdot\|_F$ means Frobenius norm that is computed as follows: $\|\mathbf{X}\|_F^2 = \sum_{i,j} x_{ij}^2$. The function $f$ is the key ingredient of the loss in matrix factorization model used in the recommender systems. The matrix $\mathbf{A}$ is binary and represents the history of user-item interactions. Note that the convexity of $f$ means that it is convex w.r.t. both arguments simultaneously.  
- ☐ $f(\mathbf{W}_1, \mathbf{W}_2) = \|\mathbf{W}_1 \max(\mathbf{W}_2 \mathbf{x}, 0)\|_2$, where max is elementwise function here. Vector $\mathbf{x}$ is given. The function inside the 2-norm is the toy instance of the DeepReLU neural network. Note that the convexity of $f$ means that it is convex w.r.t. $\mathbf{W}_1, \mathbf{W}_2$ simultaneously.  


1. **$f(\mathbf{x}) = \sup_{\mathbf{y} \in C} \langle \mathbf{y}, \mathbf{x} \rangle$**: **Convex**  
    This is a support function. Here's why it's convex: it's the supremum of linear functions, and supremum of linear functions is always convex. You can think of it as taking the highest point among all these linear functions at each $\mathbf{x}$.

2. **$f(\mathbf{x}) = \|\mathbf{A}\mathbf{x} - \mathbf{b}\|$**: **Convex**  
    Two key facts here: any norm is convex, and when we transform its argument with an affine mapping ($\mathbf{A}\mathbf{x} - \mathbf{b}$), the result stays convex. So composing these operations preserves convexity.

3. **$f(\mathbf{x}) = \min_{i=1,\dots,m} x_i$**: **Concave**  
     $\min_i x_i = -\max_i(-x_i)$. Since max of linear functions is convex, and we're negating it, our function must be concave. Another way: minimum of linear functions is always concave.

4. **$f(\mathbf{x}) = -\left(\prod_{i=1}^n x_i\right)^{1/n}$**: **Convex**  
    Inside the negative sign we have the geometric mean, which is concave on $\mathbb{R}^n_+$. When we put minus in front of a concave function, we get a convex function.

5. **$f(\mathbf{w}) = \sum_{i=1}^m \log(1 + e^{-y_i \mathbf{w}^\top \mathbf{x}_i}) + \frac{1}{2}\|\mathbf{w}\|^2$**: **Convex**  
    The logistic loss $\log(1 + e^{-z})$ is convex in $z$. Since $z = y_i \mathbf{w}^\top \mathbf{x}_i$ is linear in $\mathbf{w}$, each term is convex. Sum of convex functions is convex, and adding $\frac{1}{2}\|\mathbf{w}\|^2$ (which is convex) keeps it convex.