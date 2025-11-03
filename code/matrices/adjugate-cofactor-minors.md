# Adjugate Matrix, Cofactor Matrix and Minors

## Adjugate Matrix

```
function adjugateMatrix(M) {
	const cm = cofactorMatrix(M);
	return transpose(cm);
}
```

## Cofactor Matrix

```
function cofactor(M,r,c) {
	const m = minor(M,r,c);
	const pf = (-1)**(r+c);
	return m*pf;
}

function cofactorMatrix(M) {
	return M.map((row,rIdx) => {
		return row.map((col,cIdx) => {
			return cofactor(M,rIdx+1,cIdx+1);
		});
	});
}
```
