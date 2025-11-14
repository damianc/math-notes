# Piecewise Functions

$$
\begin{array}{ll}
f(x) = \\{
\\
& CONDITION-1: EXPR-1,
\\
& CONDITION-2: EXPR-2,
\\
& ...,
\\
& CONDITION-N: EXPR-N,
\\
& DEFAULT-EXPR
\\
\\}
\end{array}
$$

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
| | { x<-1: -x, x>1:x, 1 } |

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
| | { i=j: 1, 0 } |
