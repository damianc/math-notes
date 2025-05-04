# Vector Products

The following vectors are considered:

$$
\begin{array}{l}
\vec{a} = [a_1, a_2, a_3]
\\
\vec{b} = [b_1, b_2, b_3]
\end{array}
$$

## Multiplication by Scalar

$$
k\vec{a} = [ka_1, ka_2, ka_3]
$$

## Dot/Scalar Product

$$
\vec{a} \cdot \vec{b} = a_1b_1 + a_2b_2 + a_3b_3
$$

> generally:  
> $$\vec{a} \cdot \vec{b} = \vec{a}^{\intercal} \vec{b} = \|\vec{a}\|\|\vec{b}\| \cos\theta = \displaystyle\sum_{k=1}^{n} a_k b_k$$

> Properties of the dot product:
> - $\vec{a} \cdot \vec{a} = \| \vec{a} \|^2$
> - $\vec{a} \cdot \vec{b} = \vec{b} \cdot \vec{a}$
> - $\vec{a} \cdot (\vec{b}+\vec{c}) = \vec{a} \cdot \vec{b} + \vec{a} \cdot \vec{c}$

## Cross/Vector Product (in $\Bbb{R}^3$)

$$
\begin{array}{rl}
\vec{a} \times \vec{b} & = \begin{vmatrix}
 \vec{i} & \vec{j} & \vec{k}
 \\
 a_1 & a_2 & a_3
 \\
 b_1 & b_2 & b_3
\end{vmatrix}
\\
\ 
\\
& = [(a_2b_3-a_3b_2)]\vec{i} - [(a_1b_3-a_3b_1)]\vec{j} + [(a_1b_2-a_2b_1)]\vec{k}
\\
\ 
\\
& = [a_2b_3-a_3b_2, a_1b_3-a_3b_1, a_1b_2-a_2b_1]
\end{array}
$$

- $\vec{i}$ - the unit vector in the direction of  the **x**, i.e., $[1,0,0]$
- $\vec{j}$ - the unit vector in the direction of  the **y**, i.e., $[0,1,0]$
- $\vec{k}$ - the unit vector in the direction of  the **z**, i.e., $[0,0,1]$

> for example, vector $\vec{a} = [2,-1,3]$ can be written as $\vec{a} = 2\vec{i} - \vec{j} + 3\vec{k}$

## Outer Product

$$
a \otimes b = ab^{\intercal} = \begin{bmatrix}
 a_1b_1 & a_1b_2 & a_1b_3 & \cdots & a_1b_n
 \\
 a_2b_1 & a_2b_2 & a_2b_3 & \cdots & a_2b_n
 \\
 \vdots & \vdots & \vdots & \ddots & \vdots
 \\
 a_m b_1 & a_m b_2 & a_m b_3 & \cdots & a_m b_n
\end{bmatrix}
$$

for example:

$$
[1,2] \otimes [3,4] = [1,2] \cdot \begin{bmatrix}
3
\\
4
\end{bmatrix} = \begin{bmatrix}
3 & 4
\\
6 & 8
\end{bmatrix}
$$

## Kronecker Product

$$
A \otimes B = \begin{bmatrix}
 a_{11}B & a_{12}B & \cdots & a_{1n}B
 \\
  a_{21}B & a_{22}B & \cdots & a_{2n}B
  \\
  \vdots & \vdots & \ddots & \vdots
  \\
  a_{m1}B & a_{m2}B & \cdots & a_{mn}B
\end{bmatrix}
$$

in short:

$$
(A \otimes B)\_{ij} = a_{ij} B
$$

for example:

$$
\begin{bmatrix}
1 & 2
\\
3 & 4
\end{bmatrix} \otimes
\begin{bmatrix}
0 & 5
\\
6 & 7
\end{bmatrix} = \begin{bmatrix}
1\begin{bmatrix}
0 & 5
\\
6 & 7
\end{bmatrix} & 2\begin{bmatrix}
0 & 5
\\
6 & 7
\end{bmatrix}
\\
\ 
\\
3\begin{bmatrix}
0 & 5
\\
6 & 7
\end{bmatrix} & 4\begin{bmatrix}
0 & 5
\\
6 & 7
\end{bmatrix}
\end{bmatrix} = \left[\begin{array}{cc|cc}
0 & 5 & 0 & 10
\\
6 & 7 & 12 & 14
\\
\hline
0 & 15 & 0 & 20
\\
18 & 21 & 24 & 28
\end{array}\right]
$$

## Hadamard Product

$$
(A \odot B)\_{ij} = a_{ij} b_{ij}
$$

for example:

$$
[1,2,0] \odot [4,4,4] = [1 \cdot 4, 2 \cdot 4, 0 \cdot 4] = [4,8,0]
$$
