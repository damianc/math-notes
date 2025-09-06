# Kronecker Delta

The **Kronecker delta** is a function that checks if two variables are equal.

$$
\large
\delta_{ij} = \begin{cases}
0 & \text{if } i \neq j
\\
1 & \text{if } i = j
\end{cases}
$$

For example:

- $\delta_{11} = 1$ because $1 = 1$
- $\delta_{12} = 0$ because $1 \neq 2$

> ℹ️ **A SINGLE-ARGUMENT VARIANT**
> 
> There is a variant of the **Kronecker delta** with only one variable - $\delta_i$, which is equivalent to setting $j=0$:
>
> 
> $$
\delta_i = \delta_{i0} = \begin{cases}
0 \quad \text{if } i \neq 0
\\
1 \quad \text{if } i=0
\end{cases}
$$


## Use Examples

- entries of the $n \times n$ _identity matrix_ **I**:

$$
I_{ij} = \delta_{ij}
$$

- the _inner product_ of vectors:

$$
a \cdot b = \sum_{i,j=1}^n a_i \delta_{ij} b_j = \sum_{i=1}^n a_i b_i
$$

- the _trace_ of a _square matrix_ **M**:

$$
\text{tr}(M) = \sum_{i,j=1}^n M_{ij} \delta_{ij} = \sum_{i=1}^n M_{ii}
$$

- [the _Lagrange interpolation_](https://github.com/damianc/math-notes/blob/master/functions/lagrange-interpolation.md):

$$
P(x) = \sum_{i=1}^n y_i \left[
\prod_{j=1}^n \left(
\frac{x-x_j}{x_i-x_j}
\right)^{1-\delta_{ij}}
\right]
$$

## Kronecker Delta as a Filter

- in a sum:

$$
\sum_{i,j} f(\dots) \delta_{ij}
$$

- in a product:

$$
\prod_{i,j} f(\dots)^{\delta_{ij}}
$$

- inverse condition:

$$
1-\delta_{ij} \equiv \begin{cases}
1 & \text{if } i \neq j
\\
0 & \text{if } i = j
\end{cases}
$$
