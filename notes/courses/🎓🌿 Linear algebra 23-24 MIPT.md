---
tags:
  - course🎓
  - status/IN_PROGRESS_🌿
publish: true
author:
  - "[[👤 Елишев, Андрей Михайлович]]"
provider: "[[🏛МФТИ|MIPT]]"
platform: "[[Цифровая среда обучения - МФТИ]]"
url: https://lms.mipt.ru/course/view.php?id=4899&type=lecture
recommendation: 
family: 
connected:
  - "[[512.64  Linear algebra MOC]]"
  - "[[🎓 CC MIPT - 1 semester]]"
created: 2023-10-14 12:29
---


The task in your screenshot involves computing the nth power of a matrix A, where A is given by:

\[ A = \begin{bmatrix} \cos(\alpha) & -\sin(\alpha) \\ \sin(\alpha) & \cos(\alpha) \end{bmatrix} \]

This matrix is a rotation matrix, which represents a rotation by an angle α in the plane. To compute \( A^n \), where \( n \) is a positive integer, there are a few properties of rotation matrices and trigonometric functions that we can use to simplify the process. Here's a step-by-step guide on how to approach this computation:

### Step-by-step Solution

1. **Understand the Matrix**: The given matrix A is a rotation matrix that rotates vectors in the 2-dimensional plane by an angle α. This kind of matrix is orthogonal, and its inverse is its transpose. This property will be useful because \( A^{-1} = A^T \) for any orthogonal matrix.

2. **Matrix Multiplication Property**: When you multiply a rotation matrix by itself, you're effectively combining two rotations. So, \( A^2 \) would rotate by \( 2\alpha \), \( A^3 \) by \( 3\alpha \), and so on. In general, \( A^n \) will rotate by \( n\alpha \).

3. **Compute \( A^2 \)**: To find \( A^n \), we first compute \( A^2 \) by multiplying the matrix A by itself.
\[ A^2 = A \cdot A \]
\[ A^2 = \begin{bmatrix} \cos(\alpha) & -\sin(\alpha) \\ \sin(\alpha) & \cos(\alpha) \end{bmatrix} \cdot \begin{bmatrix} \cos(\alpha) & -\sin(\alpha) \\ \sin(\alpha) & \cos(\alpha) \end{bmatrix} \]

4. **Use Trigonometric Identities**: During the multiplication, you'll use the sum of angles identities for sine and cosine:
\[ \cos(x + y) = \cos(x)\cos(y) - \sin(x)\sin(y) \]
\[ \sin(x + y) = \sin(x)\cos(y) + \cos(x)\sin(y) \]
These identities show that the product of two rotation matrices is another rotation matrix with the sum of the angles.

5. **Inductive Step**: If we assume that \( A^k \) is a rotation by \( k\alpha \), then \( A^{k+1} = A^k \cdot A \) is a rotation by \( (k+1)\alpha \). This inductive step can be proven using the trigonometric identities mentioned above.

6. **Conclusion**: Therefore, \( A^n \) will be a rotation matrix that rotates by \( n\alpha \). So, we can write:
\[ A^n = \begin{bmatrix} \cos(n\alpha) & -\sin(n\alpha) \\ \sin(n\alpha) & \cos(n\alpha) \end{bmatrix} \]

This is the general form of the nth power of the rotation matrix A.

To demonstrate the multiplication for \( A^2 \), I can perform the matrix multiplication for you. Would you like to proceed with that?

---

The matrix B in your screenshot is of the form:

\[ B = \begin{bmatrix} \lambda & 1 \\ 0 & \lambda \end{bmatrix}^n \]

This matrix is an example of a Jordan block. When raising a Jordan block to a power \( n \), the diagonal elements, which are all \( \lambda \), will remain \( \lambda \) in \( B^n \). The off-diagonal elements (above the main diagonal) are a bit trickier, as they will change based on the power \( n \). For a 2x2 Jordan block, the (1,2) entry of \( B^n \) will be \( n\lambda^{n-1} \) when \( \lambda \neq 0 \).

Here's how you can compute \( B^n \) step by step:

### Step-by-Step Solution

1. **Matrix Squaring**: Begin by finding \( B^2 \):
\[ B^2 = B \cdot B \]
\[ B^2 = \begin{bmatrix} \lambda & 1 \\ 0 & \lambda \end{bmatrix} \cdot \begin{bmatrix} \lambda & 1 \\ 0 & \lambda \end{bmatrix} \]

2. **Perform the Multiplication**: When you multiply \( B \) by itself, the result will be:
\[ B^2 = \begin{bmatrix} \lambda^2 & \lambda + 1 \\ 0 & \lambda^2 \end{bmatrix} \]

3. **General Pattern Recognition**: Notice the pattern in the off-diagonal entry. For \( B^3 \), the (1,2) entry would be \( \lambda^2 + 2\lambda \), which suggests a pattern for the powers of B.

4. **Inductive Step**: Assume that for \( B^k \), the (1,2) entry is \( k\lambda^{k-1} \). Then for \( B^{k+1} \), the (1,2) entry will be \( k\lambda^k + \lambda^{k} \), which simplifies to \( (k+1)\lambda^k \).

5. **Conclusion**: Therefore, \( B^n \) will have the form:
\[ B^n = \begin{bmatrix} \lambda^n & n\lambda^{n-1} \\ 0 & \lambda^n \end{bmatrix} \]

This is the nth power of the matrix B.

If you'd like to see the multiplication for \( B^2 \) explicitly calculated or if you need further explanation on any of the steps, please let me know!