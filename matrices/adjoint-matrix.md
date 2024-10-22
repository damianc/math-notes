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

## JavaScript Implementation

```
function adjointMatrix(M) {
  return transpose(cofactors(M));
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
