# Lagrange Interpolation

**Lagrange interpolation** (or **polynomial interpolation**) finds a polynomial function whose graph passes through given points. That is, by a set of points $(x_1,y_1),(x_2,y_2),\dots,(x_n,y_n)$, we can find such a function $P(x)$ for which the following holds:

$$
\begin{cases}
y_1 = P(x_1)
\\
y_2 = P(x_2)
\\
\dots
\\
y_n = P(x_n)
\end{cases}
$$
  
  ## Formula

$$
\large
P(x) = \sum_{i=1}^n y_i \ell_i(x), \quad 
\ell_i(x) = \prod_{j \neq i}  \frac{x-x_j}{x_i-x_j}
$$

or with [the _Kronecker delta_](https://github.com/damianc/math-notes/blob/master/functions/specials/kronecker-delta.md):

$$
\large
P(x) = \sum_{i=1}^n y_i \left[
\prod_{j=1}^n \left(
\frac{x-x_j}{x_i-x_j}
\right)^{1-\delta_{ij}}
\right]
$$

### Related Articles

- [Finding a Line by Two Points](https://github.com/damianc/math-notes/blob/master/analytic-geometry/finding-line.md#by-two-points)
- [Finding a Parabola by Roots and Vertex](https://github.com/damianc/math-notes/blob/master/functions/quadratic/constructing-parabola.md)

## Expansion

- For two points $(x_1,y_1), (x_2,y_2)$:

$$
\begin{array}{rl}
P(x) & = y_1\left(
\frac{x-x_2}{x_1-x_2}
\right) + y_2\left(
\frac{x-x_1}{x_2-x_1}
\right)
\\
\ 
\\
& = \frac{
y_1(x-x_2)(x_2-x_1)+y_2(x-x_1)(x_1-x_2)
}{
-(x_1-x_2)^2
}
\\
\ 
\\
& = \frac{
(x_1-x_2)(y_1(x-x_2)-y_2(x-x_1))
}{
-(x_1-x_2)^2
}
\\
\ 
\\
& = \frac{
y_2(x-x_1)-y_1(x-x_2)
}{
x_2-x_1
}
\end{array}
$$

- For three points $(x_1,y_1), (x_2,y_2), (x_3,y_3)$:

$$
\begin{array}{rl}
P(x) & = y_1\left(
\frac{x-x_2}{x_1-x_2} \frac{x-x_3}{x_1-x_3}
\right) + y_2\left(
\frac{x-x_1}{x_2-x_1} \frac{x-x_3}{x_2-x_3}\right) + y_3\left(
\frac{x-x_1}{x_3-x_1} \frac{x-x_2}{x_3-x_2}
\right)
\\
\ 
\\
& = \frac{y_1(x-x_2)(x-x_3)}{(x_1-x_2)(x_1-x_3)} +
\frac{y_2(x-x_1)(x-x_3)}{(x_2-x_1)(x_2-x_3)} +
\frac{y_3(x-x_1)(x-x_2)}{(x_3-x_1)(x_3-x_2)}
\end{array}
$$

## Examples

### Example 1

Find a function that passes through points:

- $(x_1,y_1) = (2,4)$
- $(x_2,y_2) = (4,8)$

Steps to do:

- list factors:

| $y_i$ | $\ell_i(x)$ |
|--|--|
| $4$ | $\ell_1(x)$ |
| $8$ | $\ell_2(x)$ |

- evaluate $\ell_i$ factors:

$$
\begin{array}{l}
\ell_1(x) = \frac{x-x_2}{x_1-x_2} = \frac{x-4}{-2} = \frac{4-x}{2} = \frac{1}{2}(4-x)
\\
\ 
\\
\ell_2(x) = \frac{x-x_1}{x_2-x_1} = \frac{x-2}{4-2} = \frac{x-2}{2} = \frac{1}{2}(x-2)
\end{array}
$$

- put all the factors into formula:

$$
\begin{array}{rl}
P(x) & = y_1 \ell_1(x) + y_2 \ell_2(x)
\\
\ 
\\
& = \frac{4}{2}(4-x) + \frac{8}{2}(x-2)
\\
\ 
\\
& = 2(4-x) + 4(x-2)
\\
\ 
\\
& = 8-2x+4x-8
\\
\ 
\\
& = 2x
\end{array}
$$

Hence the function is:

$$
\large
P(x) = 2x
$$

### Example 2

Find a function that passes through points:

- $(x_1,y_1) = (1,3)$
- $(x_2,y_2) = (2,6)$
- $(x_3,y_3) = (4,18)$

Steps to do:

- list factors:

| $y_i$ | $\ell_i(x)$ |
|--|--|
| $3$ | $\ell_1(x)$ |
| $6$ | $\ell_2(x)$ |
| $18$ | $\ell_3(x)$ |

- evaluate $\ell_i$ factors:

$$
\begin{array}{l}
\ell_1(x) = \frac{(x-x_2)(x-x_3)}{(x_1-x_2)(x_1-x_3)} = \frac{(x-2)(x-4)}{(1-2)(1-4)} = \frac{(x-2)(x-4)}{3} = \frac{1}{3}(x-2)(x-4)
\\
\ 
\\
\ell_2(x) = \frac{(x-x_1)(x-x_3)}{(x_2-x_1)(x_2-x_3)} = \frac{(x-1)(x-4)}{(2-1)(2-4)} = \frac{(x-1)(x-4)}{-2} = -\frac{1}{2}(x-1)(x-4)
\\
\ 
\\
\ell_3(x) = \frac{(x-x_1)(x-x_2)}{(x_3-x_1)(x_3-x_2)} = \frac{(x-1)(x-2)}{(4-1)(4-2)} = \frac{(x-1)(x-2)}{6} = \frac{1}{6}(x-1)(x-2)
\end{array}
$$

- put all the factors into formula:

$$
\begin{array}{rl}
P(x) & = y_1 \ell_1(x) + y_2 \ell_2(x) + y_3 \ell_3(x)
\\
\ 
\\
& = \frac{3}{3}(x-2)(x-4) - \frac{6}{2}(x-1)(x-4) + \frac{18}{6}(x-1)(x-2)
\\
\ 
\\
& = (x-2)(x-4) - 3(x-1)(x-4) + 3(x-1)(x-2)
\\
\ 
\\
& = (x^2-6x+8) - (3x^2-15x+12) + (3x^2-9x+6)
\\
\ 
\\
& = x^2-6x+8-3x^2+15x-12+3x^2-9x+6
\\
\ 
\\
& = x^2 + 2
\end{array}
$$

Hence the function is:

$$
\large
P(x) = x^2 + 2
$$
