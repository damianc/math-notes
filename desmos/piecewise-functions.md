# Piecewise Functions

$$
\begin{array}{ll}
f(x) = \\{
\\
& \text{CONDITION-1: EXPR-1,} 
\\
& \text{CONDITION-2: EXPR-2,}
\\
& \text{...,}
\\
& \text{CONDITION-N: EXPR-N,}
\\
& \text{[DEFAULT-EXPR]}
\\
\\}
\end{array}
$$

> A _default expression_ is optional.

## Example 1

$$
f(x) = \begin{cases}
-x & \text{if } x \lt -1
\\
x & \text{if } x \gt 1
\\
1 & \text{otherwise (if } x \in [-1,1] \text{)}
\end{cases}
$$

| | |
|--|--|
| | f(x) = { x<-1: -x, x>1:x, 1 } |

## Example 2 (Kronecker Delta)

$$
d(i,j) = \begin{cases}
1 & \text{if } i=j
\\
0 & \text{otherwise}
\end{cases}
$$

| | |
|--|--|
| | d(i,j) = { i=j: 1, 0 } |
