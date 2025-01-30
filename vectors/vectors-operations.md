# Operations on Vectors

The following vectors are considered:

$$
\begin{array}{l}
\vec{a} = [a_1, a_2, a_3]
\\
\vec{b} = [b_1, b_2, b_3]
\end{array}
$$

## Sum/Difference

$$
\vec{a} \pm \vec{b} = [
 a_1 \pm b_1, a_2 \pm b_2, a_3 \pm b_3
]
$$

## Multiplication by Scalar

$$
k\vec{a} = [
 ka_1, ka_2, ka_3
]
$$

## Dot/Scalar Product

$$
\vec{a} \cdot \vec{b} = a_1 b_1 + a_2 b_2 + a_3 b_3
$$

## Cross/Vector Product (in $\Bbb{R}^3$)

$$
\vec{a} \times \vec{b} = \begin{bmatrix}
\hat{i} & \hat{j} & \hat{k}
\\
a_1 & a_2 & a_3
\\
b_1 & b_2 & b_3
\end{bmatrix} = \begin{bmatrix}
 a_2 b_3 - a_3 b_2
 \\
 a_1 b_3 - a_3 b_1
 \\
 a_1 b_2 - a_2 b_1
\end{bmatrix}^{\intercal}
$$

## Other Products

### Outer Product

$$
\vec{A} \otimes \vec{B} = P, P_{ij} = a_i b_j
$$

$$
P = \begin{bmatrix}
a_1 b_1 & a_1 b_2 & \cdots
\\
a_2 b_1 & a_2 b_2 & \cdots
\\
\vdots & \vdots & \ddots
\end{bmatrix}
$$

### Kronecker Product

$$
\vec{A} \otimes \vec{B} = K, K_{ij} = a_{ij} \vec{B}
$$

$$
K = \begin{bmatrix}
a_{11} \vec{B} & a_{12} \vec{B} & \cdots
\\
a_{21} \vec{B} & a_{22} \vec{B} & \cdots
\\
\vdots & \vdots & \ddots
\end{bmatrix}
$$

## Vector Projection

$$
\text{proj}_b \ a = \frac{a \cdot b}{|b|^2} b
$$
