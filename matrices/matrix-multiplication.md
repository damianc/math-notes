# Matrix Multiplication

- multiplication of matrices is not commutative, i.e., $AB \neq BA$
- matrices $A$ and $B$ can be multiplied only if a number of columns in $A$ equals a number of rows in $B$
- if $C$ is the resultant matrix ($A \cdot B$):
  - a number of its rows equals a number of rows in $A$
  - a number of its columns equals a number of columns in $B$

$$
\large
A_{m \times n} \cdot B_{n \times p} = C_{m \times p}
$$

## JavaScript Implementation

```
function multiply(A,B) {
  const colsA = A[0].length;
  const rowsB = B.length;
  if (colsA !== rowsB) {
    throw new Error('incompatible matrices');
  }
 
  const rowsA = A.length;
  const colsB = B[0].length;
  const C = initNullMatrix(rowsA,colsB);
 
  for (let i=0; i<rowsA; i++) {
    for (let j=0; j<colsB; j++) {
      let sum = 0;
      for (let k=0; k<colsA; k++) {
        sum += A[i][k] * B[k][j];
      }
      C[i][j] = sum;
    }
  }

  return C;
}

function initNullMatrix(m,n) {
  const M = [];
  for (let i=1; i<=m; i++) {
    M.push((new Array(n)).fill(0));
  }
  return M;
}
```

