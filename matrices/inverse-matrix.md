# Inverse Matrix

Inverse matrix of matrix $A$ is its [adjoint matrix](https://github.com/damianc/math-notes/blob/master/matrices/adjoint-matrix.md) divided by its determinant.

$$
\large
A^{-1} = {\small\frac{1}{\det A}}\ \overline{A} = {\small\frac{1}{\det A}}\ A_c
$$

## Steps to Obtain Inverse Matrix

1. Let $M$ be the original matrix
2. Find its [cofactors matrix](https://github.com/damianc/math-notes/blob/master/matrices/matrix-cofactors.md) $M_c$
3. Transpose the cofactors matrix to get [adjoint matrix](https://github.com/damianc/math-notes/blob/master/matrices/adjoint-matrix.md) $\overline{M} = M_c^T$
4. Divide the adjoint matrix $\overline{M}$ by the determinant of the original matrix $M$
