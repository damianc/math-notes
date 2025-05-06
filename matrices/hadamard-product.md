# Hadamard Product

The **Hadamard product** multiplies corresponding terms of a matrix.

> the **Hadamard product** is denoted by $A \odot B$ (sometimes $A \circ B$)

If $M = A \odot B$, then:

$$
M_{ij} = A_{ij} \cdot B_{ij}
$$

## Examples

### Example 1

$$
\begin{bmatrix}
1 & 2
\\
3 & 4
\end{bmatrix} \odot \begin{bmatrix}
10 & 4
\\
0 & 1
\end{bmatrix} = \begin{bmatrix}
10 & 8
\\
0 & 4
\end{bmatrix}
$$

### Example 2

- if a matrix of transformation $T$ is as follows:

$$
T = \begin{bmatrix}
2 & \pi & 0
\\
\pi & 2 & 0
\\
0 & 0 & 1
\end{bmatrix}
$$

- and a matrix-mask $R$ to reset the rotation is as follows:

$$
R = \begin{bmatrix}
1 & 0 & 1
\\
0 & 1 & 1
\\
0 & 0 & 1
\end{bmatrix}
$$

- a matrix of transformation with the rotation reset is as follows:

$$
T \odot R = \begin{bmatrix}
2 & 0 & 0
\\
0 & 2 & 0
\\
0 & 0 & 1
\end{bmatrix}
$$

### Example 3

This time values will be reset to a non-zero value.

- if a matrix of transformation $T$ is as follows:

$$
T = \begin{bmatrix}
2 & \pi & 0
\\
\pi & 2 & 0
\\
0 & 0 & 1
\end{bmatrix}
$$

- and a matrix-mask $R$ to reset the scaling is as follows:

$$
R = \begin{bmatrix}
0 & 1 & 1
\\
1 & 0 & 1
\\
0 & 0 & 1
\end{bmatrix}
$$

- and an additional matrix of default values $D$ is as follows:

$$
D = \begin{bmatrix}
1 & 0 & 0
\\
0 & 1 & 0
\\
0 & 0 & 0
\end{bmatrix}
$$

- a matrix of transformation with the scaling reset is as follows:

$$
(T \odot R) + D  = \begin{bmatrix}
1 & \pi & 0
\\
\pi & 1 & 0
\\
0 & 0 & 1
\end{bmatrix}
$$
