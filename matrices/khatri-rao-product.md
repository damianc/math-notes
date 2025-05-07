# Khatri-Rao Product

The **Khatri-Rao product** (or _block Kronecker product_) of two partitioned matrices $A$ and $B$ is defined as:

$$
A * B = (A_{ij} \otimes B_{ij})_{ij}
$$

in which the ij-th block is the $m_i p_i \times n_j q_j$ sized [Kronecker product](https://github.com/damianc/math-notes/blob/master/matrices/kronecker-product.md) of the corresponding blocks of $A$ and $B$, assuming the number of row and column partitions of both matrices is equal. The size of the product is then $(\Sigma_i m_i p_i) \times (\Sigma_j n_j q_j)$.

$$
\left[\begin{array}{c|c}
A_{11} & A_{12}
\\
\hline
A_{21} & A_{22}
\end{array}\right] * \left[\begin{array}{c|c}
B_{11} & B_{12}
\\
\hline
B_{21} & B_{22}
\end{array}\right]
$$

$$
= \left[\begin{array}{c|c}
A_{11} \otimes B_{11} & A_{12} \otimes B_{12}
\\
\hline
A_{21} \otimes B_{21} & A_{22} \otimes B_{22}
\end{array}\right]
$$

> each partition in the example above is a partition in a corresponding corner of the [Tracy-Singh product](https://github.com/damianc/math-notes/blob/master/matrices/tracy-singh-product.md)

## Example

If matrices $A$ and $B$ are defined as follows:

$$
A = \left[\begin{array}{c|c}
A_{11} & A_{12}
\\
\hline
A_{21} & A_{22}
\end{array}\right] = \left[\begin{array}{cc|c}
1 & 2 & 3
\\
4 & 5 & 6
\\
\hline
7 & 8 & 9
\end{array}\right]
$$

$$
B = \left[\begin{array}{c|c}
B_{11} & B_{12}
\\
\hline
B_{21} & B_{22}
\end{array}\right] = \left[\begin{array}{c|cc}
\alpha & \beta & \gamma
\\
\hline
\delta & \theta & \varphi
\\
\lambda & \mu & \omega
\end{array}\right]
$$

Then:

$$
A * B = \left[\begin{array}{c|c}
A_{11} \otimes B_{11} & A_{12} \otimes B_{12}
\\
\hline
A_{21} \otimes B_{21} & A_{22} \otimes B_{22}
\end{array}\right]
$$

$$
= \left[\begin{array}{cc|cc}
\alpha & 2\alpha & 3\beta & 3\gamma
\\
4\alpha & 5\alpha & 6\beta & 6\gamma
\\
\hline
7\delta & 8\delta & 9\theta & 9\varphi
\\
7\lambda & 8\lambda & 9\mu & 9\omega
\end{array}\right]
$$

## Column-Wise Kronecker Product

The **column-wise Kronecker product** of two matrices is a special case of the **Khatri-Rao product** as defined above, and may also be called the _Khatri-Rao product_.

This product assumes the partitions of the matrices are their columns. In this case $m_1 = m$, $p_1 = p$, $n=q$ and $\forall_j \ n_j = q_j = 1$.

The resulting product is a $mp \times n$ matrix of which each column is the [Kronecker product](https://github.com/damianc/math-notes/blob/master/matrices/kronecker-product.md) of the corresponding columns of $A$ and $B$.

### Example

If matrices $A$ and $B$ are defined as follows:

$$
A = [A_1 | A_2 | A_3 ] = \left[\begin{array}{c|c|c}
1 & 2 & 3
\\
4 & 5 & 6
\\
7 & 8 & 9
\end{array}\right]
$$

$$
B = [B_1 | B_2 | B_3 ] = \left[\begin{array}{c|c|c}
\alpha & \delta & \lambda
\\
\beta & \theta & \mu
\\
\gamma & \varphi & \omega
\end{array}\right]
$$

Then:

$$
A * B = [ A_1 \otimes B_1 \ | \ A_2 \otimes B_2 \ | \ A_3 \otimes B_3 ]
$$

$$
= \left[\begin{array}{c|c|c}
\alpha & 2\delta & 3\lambda
\\
\beta & 2\theta & 3\mu
\\
\gamma & 2\varphi & 3\omega
\\
4\alpha & 5\delta & 6\lambda
\\
4\beta & 5\theta & 6\mu
\\
4\gamma & 5\varphi & 6 \omega
\\
7\alpha & 8\delta & 9\lambda
\\
7\beta & 8\theta & 9\mu
\\
7\gamma & 8\varphi & 9\omega
\end{array}\right]
$$
