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

## Minors

```
function minorize(M,r,c) {
	return removeRow(removeCol(M,c),r);
}

function minor(M,r,c) {
	return det(minorize(M,r,c));
}

function minorMatrix(M) {
	return M.map((row,rIdx) => {
		return row.map((col,cIdx) => {
			return minor(M,rIdx+1,cIdx+1);
		});
	});
}
```

## Version with Matrix Mapper

```
function cofactorMatrix(M) {
	return mapTerms(
		M, (_,r,c) => cofactor(M,r,c)
	);
}

function minorMatrix(M) {
	return mapTerms(
		M, (_,r,c) => minor(M,r,c)
	);
}
```

Arguments passed to a callback of the following mapper are as follows:
- current matrix term
- a number of a row (starting from 1)
- a number of a column (starting from 1)
- an overall number of a matrix term (starting from 1)

```
function mapTerms(M, cb) {
	const rows = M.length;
	const cols = M[0].length;
	const N = [];
	let numOfTerm = 1;
	for (let ri=0; ri<rows; ri++) {
		N.push([]);
		for (let ci=0; ci<cols; ci++) {
			const nv = cb(
				M[ri][ci], ri+1, ci+1, numOfTerm++
			);
			N[ri].push(nv);
		}
	}
	return N;
}
```
