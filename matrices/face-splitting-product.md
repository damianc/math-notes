# Face-Splitting Product

The **face-splitting product** (or _transposed Khatri-Rao product_) produces a matrix in such a way that element $a_{ij}$ multiplies i-th row of the matrix $B$.

$$
A \mathop{\small\square} B = \bigl[
a_{ij} \cdot B_i
\bigr]
$$

It can be defined in terms of the **Kronecker product** as:

$$
\begin{bmatrix}
A_1
\\
\hline
A_2
\\
\hline
\vdots
\\
\hline
A_n
\end{bmatrix} \bullet \begin{bmatrix}
B_1
\\
\hline
B_2
\\
\hline
\vdots
\\
\hline
B_n
\end{bmatrix} = \begin{bmatrix}
A_1 \otimes B_1
\\
\hline
A_2 \otimes B_2
\\
\hline
\vdots
\\
\hline
A_n \otimes B_n
\end{bmatrix}
$$

## Example

If matrices $A$ and $B$ are defined as follows:

$$
A = \begin{bmatrix}
1 & 2
\\
3 & 4
\\
5 & 6
\end{bmatrix}
$$

$$
B = \begin{bmatrix}
\alpha & \beta & \gamma
\\
\delta & \theta & \varphi
\\
\lambda & \mu & \omega
\end{bmatrix}
$$

Then:

$$
A \mathop{\small\square} B = \begin{bmatrix}
1 \cdot [\alpha \ \beta \ \gamma] & 2 \cdot [\alpha \ \beta \ \gamma]
\\
3 \cdot [\delta \ \theta \ \varphi] & 4 \cdot [\delta \ \theta \ \varphi]
\\
5 \cdot [\lambda \ \mu \ \omega] & 6 \cdot [\lambda \ \mu \ \omega]
\end{bmatrix}
$$

$$
= \begin{bmatrix}
\alpha & \beta & \gamma & 2\alpha & 2\beta & 2\gamma
\\
3\delta & 3\theta & 3\varphi & 4\delta & 4\theta & 4\varphi
\\
5\lambda & 5\mu & 5\omega & 6\lambda & 6\mu & 6\omega
\end{bmatrix}
$$
