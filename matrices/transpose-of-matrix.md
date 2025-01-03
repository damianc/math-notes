# Transpose of a Matrix

The transpose $A^T$ of a matrix $A$ is a matrix that contains elements of $A$ but with switched the row and column indices, i.e., element $a_{ji}$ in $A$ becomes element $a_{ij}$ in $A^T$:

$$
[A^T]\_{ij} = [A]_{ji}
$$

In other words, the rows of $A$ are written as the columns of $A^T$, or - what gives the same effect - the columns of $A$ are written as the rows of $A^T$. 

Hence, if $A$ is a matrix $m \times n$, then $A^T$ is a matrix $n \times m$.

## Examples

$$
\begin{array}{ll}
A = \begin{bmatrix}
1 & 2
\\
3 & 4
\\
5 & 6
\end{bmatrix}
&
A^T = \begin{bmatrix}
1 & 3 & 5
\\
2 & 4 & 6
\end{bmatrix}
\\
\ 
\\
B = \begin{bmatrix}
1 & 2
\\
3 & 4
\end{bmatrix}
&
B^T = \begin{bmatrix}
1 & 3
\\
2 & 4
\end{bmatrix}
\\
\ 
\\
C = \begin{bmatrix}
1 & 2 & 3
\end{bmatrix}
&
C^T = \begin{bmatrix}
1
\\
2
\\
3
\end{bmatrix}
\\
\ 
\\
D = \begin{bmatrix}
1
\\
2
\end{bmatrix}
&
D^T = \begin{bmatrix}
1 & 2
\end{bmatrix}
\end{array}
$$
