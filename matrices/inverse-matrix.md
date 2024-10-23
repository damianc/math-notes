# Inverse Matrix

Inverse matrix of matrix $A$ is its [adjoint matrix](https://github.com/damianc/math-notes/blob/master/matrices/adjoint-matrix.md) divided by its determinant.

$$
\large
A^{-1} = {\small\frac{1}{\det A}}\ \overline{A} = {\small\frac{1}{\det A}}\ A_c^T
$$

## Steps to Obtain Inverse Matrix

1. Let $M$ be the original matrix:

$$
M = \begin{bmatrix}
1 & 2
\\
3 & 4
\end{bmatrix}
$$

2. Find its [cofactors matrix](https://github.com/damianc/math-notes/blob/master/matrices/matrix-cofactors.md) $M_c$:

$$
M_c = \begin{bmatrix}
M_{11} & -M_{12}
\\
-M_{21} & M_{22}
\end{bmatrix} = \begin{bmatrix}
4 & -3
\\
-2 & 1
\end{bmatrix}
$$

3. Transpose the cofactors matrix to get [adjoint matrix](https://github.com/damianc/math-notes/blob/master/matrices/adjoint-matrix.md) $\overline{M} = M_c^T$:

$$
\overline{M} = M_c^T = \begin{bmatrix}
4 & -2
\\
-3 & 1
\end{bmatrix}
$$

4. Divide the adjoint matrix $\overline{M}$ by the [determinant](https://github.com/damianc/math-notes/blob/master/matrices/matrix-determinant.md) of the original matrix $M$:

$$
\begin{array}{rrl}
\because & \det M & = \begin{vmatrix}
1 & 2
\\
3 & 4
\end{vmatrix}
\\
& & = 1 \cdot 4 - 2 \cdot 3 = -2
\\
\ 
\\
\therefore & M^{-1} & = \frac{1}{\det M}\ \overline{M}
\\
& & = \frac{1}{-2}\ \begin{bmatrix}
4 & -2
\\
-3 & 1
\end{bmatrix}
\\
& & = \begin{bmatrix}
-2 & 1
\\
1.5 & -0.5
\end{bmatrix}
\end{array}
$$
