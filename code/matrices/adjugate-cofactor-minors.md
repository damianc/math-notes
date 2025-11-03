# Adjugate Matrix, Cofactor Matrix and Minors

## Adjugate Matrix

```
function adjugateMatrix(M) {
	const cm = cofactorMatrix(M);
	return transpose(cm);
}
```
