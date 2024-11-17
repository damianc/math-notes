# Polylogarithm Function

$$
\Large
\text{Li}\_n(x) = \sum_{k=1}^{\infty}
\frac{x^k}{k^n}
$$

## JavaScript Implementation

```
function Li(n,x,iters=100) {
  const precision = 1e-10;
  let sum = 0;
  
  for (let k=1; k<iters; k++) {
    const term = (x**k)/(k**n);
    sum += term;
    if (Math.abs(term) < precision) break;
  }
  
  return sum;
}
```
