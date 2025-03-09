# Newton Interpolation

The **Newton interpolation** finds a function  $P_k(x)$ by a set of points $(x_1,y_1),(x_2,y_2),\dots,(x_k,y_k), (x_{k+1},y_{k+1})$ it passes through.

> $k$ in the name of a function - $P_k(x)$ - is a number of points decreased by one

Such a function is defined as:

$$
P_k(x) = \Delta^0_1 + \sum_{r=1}^k \Delta^r_1 \cdot \prod_{i=1}^r x-x_i
$$

which expands to:

$$
\begin{array}{rl}
P_k(x) = & \Delta^0_1 \ +
\\
& \Delta^1_1(x-x_1) \ +
\\
& \Delta^2_1(x-x_1)(x-x_2) \ +
\\
& \cdots \ +
\\
& \Delta^k_1(x-x_1)(x-x_2)\cdots(x-x_k)
\end{array}
$$

where $\Delta^n_1$ is a specific factor - _divided difference_, which can be written out in _a triangular table_:

$$
\begin{array}{l|lllcll}
x_i & y_i = \Delta^0_i & \Delta^1_i & \Delta^2_i & \cdots & \Delta^{k-1}\_i & \Delta^k_i
\\
\ 
\\
\hline
\\
x_1 & y_1 & \Delta^1_1 & \Delta^2_1 & \cdots & \Delta^{k-1}\_1 & \Delta^k_1
\\
\ 
\\
x_2 & y_2 & \Delta^1_2 & \Delta^2_2 & \cdots & \Delta^{k-1}\_2
\\
\ \ \vdots & \ \ \vdots & \ \ \vdots & \ \ \vdots & \large\cdot^{\large\cdot^{\large\cdot}}
\\
x_{k-1} & y_{k-1} & \Delta^1_{k-1} & \Delta^2_{k-1}
\\
\ 
\\
x_k & y_k & \Delta^1_k
\\
\ 
\\
x_{k+1} & y_{k+1}
\end{array}
$$

where $\Delta^k_i$ is as follows:

$$
\Delta^k_i = \frac{
\Delta^{k-1}\_{i+1} - \Delta^{k-1}\_i
}{
x_{i+k} - x_i
}, \ \ \Delta^0_i = y_i
$$

## Examples

### Example 1

Find a function that passes through points:
- $(x_1,y_1) = (1,3)$
- $(x_2,y_2) = (2,6)$
- $(x_3,y_3) = (4,18)$

Steps to do:

- initiate a table of the divided differences:

$$
\begin{array}{c|ccc}
x_i & y_i & \Delta^1_i & \Delta^2_i
\\
\hline
1 & 3 & \Delta^1_1 & \Delta^2_1
\\
2 & 6 & \Delta^1_2
\\
4 & 18
\end{array}
$$

- evaluate factors:

$$
\begin{array}{l}
\Delta^1_1 = \frac{y_2-y_1}{x_2-x_1} = \frac{6-3}{2-1} = \frac{3}{1} = 3
\\
\ 
\\
\Delta^1_2 = \frac{y_3-y_2}{x_3-x_2} = \frac{18-6}{4-2} = \frac{12}{2} = 6
\\
\ 
\\
\Delta^2_1 = \frac{\Delta^1_2-\Delta^1_1}{x_3-x_1} = \frac{6-3}{4-1} = \frac{3}{3} = 1
\end{array}
$$

- put them into the table:

$$
\begin{array}{c|ccc}
x_i & y_i & \Delta^1_i & \Delta^2_i
\\
\hline
1 & 3 & 3 & 1
\\
2 & 6 & 6
\\
4 & 18
\end{array}
$$

- take terms from the first row:

$$
\begin{array}{ccc}
y_i & \Delta^1_i & \Delta^2_i
\\
\hline
3 & 3 & 1
\end{array}
$$

- put them into formula:

$$
\begin{array}{rl}
P_2(x) & = y_1 + \Delta^1_1(x-x_1) + \Delta^2_1(x-x_1)(x-x_2)
\\
& = 3 + 3(x-x_1) + (x-x_1)(x-x_2)
\end{array}
$$

- insert values of $x_i$:

$$
P_2(x) = 3 + 3(x-1) + (x-1)(x-2)
$$

- simplify the expression:

$$
\begin{array}{rl}
P_2(x) & = 3 + 3(x-1) + (x-1)(x-2)
\\
& = 3+3x-3+x^2-3x+2
\\
& = x^2+2
\end{array}
$$

Hence the function is:

$$
\large
P_2(x) = x^2 + 2
$$

### Example 2

Find a function that passes through points:
- $(x_1,y_1) = (2,3)$
- $(x_2,y_2) = (3,9)$
- $(x_3,y_3) = (4,19)$
- $(x_4,y_4) = (5,33)$

Steps to do:

- initiate a table of the divided differences:

$$
\begin{array}{c|ccc}
x_i & y_i & \Delta^1_i & \Delta^2_i & \Delta^3_i
\\
\hline
2 & 3 & \Delta^1_1 & \Delta^2_1 & \Delta^3_1
\\
3 & 9 & \Delta^1_2 & \Delta^2_2
\\
4 & 19 & \Delta^1_3
\\
5 & 33
\end{array}
$$

- evaluate factors:

$$
\begin{array}{l}
\Delta^1_1 = \frac{y_2-y_1}{x_2-x_1} = \frac{9-3}{3-2} = \frac{6}{1} = 6
\\
\ 
\\
\Delta^1_2 = \frac{y_3-y_2}{x_3-x_2} = \frac{19-9}{4-3} = \frac{10}{1} = 10
\\
\ 
\\
\Delta^1_3 = \frac{y_4-y_3}{x_4-x_3} = \frac{33-19}{5-4} = \frac{14}{1} = 14
\\
\ 
\\
\Delta^2_1 = \frac{\Delta^1_2-\Delta^1_1}{x_3-x_1} = \frac{10-6}{4-2} = \frac{4}{2} = 2
\\
\ 
\\
\Delta^2_2 = \frac{\Delta^1_3-\Delta^1_2}{x_4-x_2} = \frac{14-10}{5-3} = \frac{4}{2} = 2
\\
\ 
\\
\Delta^3_1 = \frac{\Delta^2_2-\Delta^2_1}{x_4-x_1} = \frac{2-2}{5-2} = \frac{0}{3} = 0
\end{array}
$$

- put them into the table:

$$
\begin{array}{c|ccc}
x_i & y_i & \Delta^1_i & \Delta^2_i & \Delta^3_i
\\
\hline
2 & 3 & 6 & 2 & 0
\\
3 & 9 & 10 & 2
\\
4 & 19 & 14
\\
5 & 33
\end{array}
$$

- take terms from the first row:

$$
\begin{array}{ccc}
y_i & \Delta^1_i & \Delta^2_i & \Delta^3_i
\\
\hline
3 & 6 & 2 & 0
\end{array}
$$

- put them into formula:

$$
\begin{array}{rl}
P_3(x) & = y_1 + \Delta^1_1(x-x_1) + \Delta^2_1(x-x_1)(x-x_2) + \Delta^3_1(x-x_1)(x-x_2)(x-x_3)
\\
& = 3 + 6(x-x_1) + 2(x-x_1)(x-x_2)
\end{array}
$$

- insert values of $x_i$:

$$
P_3(x) = 3 + 6(x-2) + 2(x-2)(x-3)
$$

- simplify the expression:

$$
\begin{array}{rl}
P_3(x) & = 3 + 6(x-2) + 2(x-2)(x-3)
\\
& = 3+6x-12+2x^2-10x+12
\\
& = 2x^2-4x+3
\end{array}
$$

Hence the function is:

$$
\large
P_3(x) = 2x^2 - 4x + 3
$$
