# Tetration

`tet(a,n)` = $\ ^n a$

```
function tet(a,n) {
  if (n === 0) return 1;

  let res = a;
  while (--n) res = a**res;
  return res;
}
```
