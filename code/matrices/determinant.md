# Matrix Determinant

```
function det(M,rowPos=1) {
	const rows = M.length;
	const cols = M[0].length;

	if (rows !== cols) return NaN;
	if (rows === 1) return M[0][0];
	if (rows === 2) {
		const [[a,b],[c,d]] = M;
		return a*d-b*c;
	}

	// Laplace expansion
	const row = M[rowPos-1];
	let res = 0;
	for (let i=0; i<row.length; i++) {
		const pf = (-1)**i;
		const val = row[i];
		const m = minor(M,rowPos,i+1);
		res += pf * val * m;
	}
	return res;
}
```
