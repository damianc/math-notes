# Adjoint Matrix

Adjoint matrix is transposed [matrix of cofactors](https://github.com/damianc/math-notes/blob/master/matrices/matrix-cofactors.md).

$$
\begin{array}{rl}
\overline{A} = A_c^T & = \begin{bmatrix}
C_{11} & C_{12} & \cdots
\\
C_{21} & C_{22} & \cdots
\\
\vdots & \vdots & \ddots
\end{bmatrix}^T
\\
\ 
\\
& = \begin{bmatrix}
C_{11} & C_{21} & \cdots
\\
C_{12} & C_{22} & \cdots
\\
\vdots & \vdots & \ddots
\end{bmatrix}
\end{array}
$$

## Example

- for matrix $A$:

$$
A = \begin{bmatrix}
1 & 2
\\
3 & 4
\end{bmatrix}
$$

- cofactor matrix $A_c$ is:

$$
A_c = \begin{bmatrix}
1 \cdot |4| & (-1) \cdot |3|
\\
(-1) \cdot |2| & 1 \cdot |1|
\end{bmatrix} = \begin{bmatrix}
4 & -3
\\
-2 & 1
\end{bmatrix}
$$

- adjoint matrix $\overline{A}$ is transposed matrix of cofactors $A_c$:

$$
\overline{A} = A_c^T = \begin{bmatrix}
4 & -2
\\
-3 & 1
\end{bmatrix}
$$

## JavaScript Implementation

```
function adjointMatrix(M) {
  return transpose(
    cofactors(M)
  );
}

function transpose(M) {
  const T = [];
  for (let i=0; i<M[0].length; i++) {
    let R = [];
    for (let j=0; j<M.length; j++) {
      R.push(M[j][i]);
    }
    T.push(R);
  }
  return T;
}
```

> [`cofactors()`](https://github.com/damianc/math-notes/blob/master/matrices/matrix-cofactors.md#javascript-implementation)
