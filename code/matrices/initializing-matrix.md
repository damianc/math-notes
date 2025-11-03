# Init Matrix

## General Matrix

> **initMatrix**(
> $\quad$ rows: int$^{+}$,
> $\quad$ cols: int$^{+}$,
> $\quad$ val: any | (int$^{+}$, int$^{+}$, uint) => any
>): any[][]

`val` can be a scalar value or a function that takes the following parameters: _row_, _column_ and _index_; first two are counted from 1, the last - from 0.

```
function initMatrix(rows,cols=rows,v=0) {
	if (rows <= 0 || cols <= 0) return;
	const M = [];
	if (typeof v !== 'function') {
	 for (let i=1; i<=rows; i++) {
		 M.push(
			 (new Array(cols)).fill(v)
		 );
	 }
	} else {
		let idx = 0;
		for (let r=1; r<=rows; r++) {
			const row = [];
			for (let c=1; c<=cols; c++) {
				row.push(v(r,c,idx++));
			}
			M.push(row);
		}
	}
	return M;
}
```

## Square Matrix

> **initSquareMatrix**(
> $\quad$ size: int$^{+}$,
> $\quad$ val: any | (int$^{+}$, int$^{+}$, uint, boolean, boolean) => any
> ): any[][]

`val` can be a scalar value or a function that takes the following parameters: _row_, _column_ (both are counted from 1), _index_ (counted from 0), and two boolean values indicating whether a term lays on _diagonal_, and next - on _anti-diagonal_.

```
function _value(v, args) {
	if (typeof v === 'function') {
		return v(...args);
	} else {
		return v;
	}
}

function initSquareMatrix(size,v=1) {
	return initMatrix(
		size,
		size,
		(r,c,i) => {
				const d = (r === c); 
				const ad = (c === size-r+1);
				return _value(v,[r,c,i,d,ad]);
		}
	);
}
```

## Diagonal Matrix

> **initDiagonalMatrix**(
> $\quad$ size: int$^{+}$,
> $\quad$ val: any | (int$^{+}$, int$^{+}$, uint) => any
> ): any[][]

```
function initDiagonalMatrix(size,v=1) {
	return initSquareMatrix(
		size,
		(r,c,i,d) => {
			if (!d) return 0;
			return _value(v,[r,c,i]);
		}
	);
}
```

## Scalar Matrix

> **initScalarMatrix**(
> $\quad$ size: int$^{+}$,
> $\quad$ val: any
> ): any[][]

```
function initScalarMatrix(size,v=1) {
	return initDiagonalMatrix(size,() => v);
}
```

## Unit Matrix

> **initUnitMatrix**(
> $\quad$ size: int$^{+}$
> ): (0|1)[][]

```
function initUnitMatrix(size) {
	return initScalarMatrix(size,1);
}
```
