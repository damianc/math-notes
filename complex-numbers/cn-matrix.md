# Complex Number in Matrix

$$
M = \begin{bmatrix}
2+i & 1+4i
\\
2+2i & 5i
\end{bmatrix}
$$

- trace:

$$
(2+i) + (0+5i) = 2+6i
$$

- determinant:

$$
\begin{array}{rl}
\det M & = (2+i)(0+5i)-(1+4i)(2+2i)
\\
& = \bigl[ 0-5+10i \bigr] - \bigl[ 2-8+(2+8)i \bigr]
\\
& = (-5+10i)-(-6+10i)
\\
& = -5+10i-10i+6
\\
& = 1
\end{array}
$$

- minor matrix:

$$
\hat{M} = \begin{bmatrix}
5i & 2+2i
\\
1+4i & 2+i
\end{bmatrix}
$$

- cofactor matrix:

$$
M_c = \begin{bmatrix}
5i & -(2+2i)
\\
-(1+4i) & 2+i
\end{bmatrix} = \begin{bmatrix}
5i & -2-2i
\\
-1-4i & 2+i
\end{bmatrix}
$$

- adjoint matrix:

$$
\overline{M} = \begin{bmatrix}
5i & -1-4i
\\
-2-2i & 2+i
\end{bmatrix}
$$

- inverse matrix:

$$
M^{-1} = \frac{1}{\det M} \ \overline{M} = \begin{bmatrix}
5i & -1-4i
\\
-2-2i & 2+i
\end{bmatrix}
$$
