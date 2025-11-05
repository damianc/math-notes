# Matrix Multiplication

To perform matrix multiplication, a number of columns of matrix A must equal a number of rows of matrix B:

> columns(A) = rows(B)

- $A_{m \times n} \cdot B_{n \times p} = C_{m \times p}$
- $C_{ij} = \displaystyle\sum_{k=1}^n A_{ik} \cdot B_{kj}$


```
function mul(A,B) {
	const aCols = A[0].length;
	const bRows = B.length;
	if (aCols !== bRows) return null;
	const L = (row,col) => {
		return row.reduce((acc,curr,idx) => {
			return acc + curr * col[idx];
		}, 0);
	};
	const M = [];
	const aRows = A.length;
	const bCols = B[0].length;
	for (let r=1; r<=aRows; r++) {
		const row = [];
		for (let c=1; c<=bCols; c++) {
			row.push(L(
				getRow(A,r), getColumn(B,c)
			));
		}
		M.push(row);
	}
	return M;
}

function getRow(M,i=1) {
	if (i >= 1 && i <= M.length) {
	 return [...M[i-1]];
	}
}

function getColumn(M,j=1) {
	if (j >= 1 && j <= M[0].length) {
	 return M.map(row => row[j-1]);
	}
}
```
