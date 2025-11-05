# Matrix Concatenation

```
function concat(A,B,h=true) {
	if (h) return concatH(A,B);
	return concatV(A,B);
}

function concatH(A,B) {
	A = [...A];
	B = [...B];
	const aRows = A.length;
	const bRows = B.length;
	const diff = Math.abs(aRows-bRows);
	if (diff > 0) {
		let M = A, N = B;
		if (aRows > bRows) [M,N] = [N,M];
		M = extendTo(M,N.length,M[0].length);
		return concatH(A,B);
	}
	const bCols = B[0].length;
	for (let i=1; i<=bCols; i++) {
		const ic = getColumn(B,i);
		addCol(A,ic);
	}
	return A;
}

function concatV(A,B) {
	A = [...A];
	B = [...B];
	const aCols = A[0].length;
	const bCols = B[0].length;
	const diff = Math.abs(aCols-bCols);
	if (diff > 0) {
		let M = A, N = B;
		if (aCols > bCols) [M,N] = [N,M];
		M = extendTo(M,M.length,N[0].length);
		return concatV(A,B);
	}
	const bRows = B.length;
	for (let i=1; i<=bRows; i++) {
		const ir = getRow(B,i);
		addRow(A,ir);
	}
	return A;
}

function extendTo(M,m,n) {
	const rows = M.length;
	const cols = M[0].length;
	const nRows = m-rows;
	const nCols = n-cols;
	if (nRows >= 0 && nCols >= 0) {
		const l = Math.max(m,n);
		for (let i=1; i<=l; i++) {
			if (i <= nRows) addRow(M);
			if (i <= nCols) addCol(M);
		}
	}
	return M;
}
```
