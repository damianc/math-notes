# Kronecker Delta

The **Kronecker delta** is a function that checks if two variables are equal.

$$
\delta_{ij} = \begin{cases}
0 & \text{if } i \neq j
\\
1 & \text{if } i = j
\end{cases}
$$

For example:

- $\delta_{11} = 1$ because $1 = 1$
- $\delta_{12} = 0$ because $1 \neq 2$

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
