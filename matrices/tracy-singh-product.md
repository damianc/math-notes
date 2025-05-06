# Tracy-Singh Product

Basically the **Tracy-Singh product** is the pairwise _Kronecker product_ for each pair of partitions in two matrices.

Its definition is as follows:

$$
A \circ B = (A_{ij} \circ B)\_{ij} = \bigl( (A_{ij} \otimes B_{kl})\_{kl} \bigr)_{ij}
$$

> "which means that the (ij)-th subblock of the $mp \times nq$ product $A \circ B$ is the $m_i p \times n_j q$ matrix $A_{ij} \circ B$ of which the (kl)-th subblock equals the $m_i p_k \times n_j q_l$ matrix $A_{ij} \otimes B_{kl}$" - as Wikipedia reads

Simply put:
- $A \circ B = (\text{every block of } A) \circ B$ (i.e., $A_{ij} \circ B$)
- $A_{ij} \circ B = (\text{block } A_{ij}) \otimes (\text{every block of } B)$

## Example

There are two matrices:

$$
A = [ A_{11} \ | \ A_{12} ] = [ 1 \ \ 2 \ | \ 4 ]
$$

$$
B = \begin{bmatrix}
B_{11}
\\
\hline
B_{21}
\end{bmatrix} = \begin{bmatrix}
\alpha & \beta
\\
\hline
\theta & \varphi
\end{bmatrix}
$$

Then:

- $A \circ B = (\text{every block of } A) \circ B$ (i.e., $A_{ij} \circ B$)

$$
A \circ B = [ A_{11} \circ B \ | \ A_{12} \circ B ]
$$

- $A_{ij} \circ B = (\text{block } A_{ij}) \otimes (\text{every block of } B)$

$$
= \left[\begin{array}{c|c}
A_{11} \otimes B_{11} & A_{12} \otimes B_{11}
\\
\hline
A_{11} \otimes B_{21} & A_{12} \otimes B_{21}
\end{array}\right]
$$

- with explicit terms:

$$
= \left[\begin{array}{c|c}
[1 \ \ 2] \otimes [\alpha \ \ \beta] & [4] \otimes [\alpha \ \ \beta]
\\
\hline
[1 \ \ 2] \otimes [\theta \ \ \varphi] & [4] \otimes [\theta \ \ \varphi]
\end{array}\right]
$$

- which means:

$$
= \left[\begin{array}{cc|c}
1 \cdot [\alpha \ \ \beta] & 2 \cdot [\alpha \ \ \beta] & 4 \cdot [\alpha \ \ \beta]
\\
\hline
1 \cdot [\theta \ \ \varphi] & 2 \cdot [\theta \ \ \varphi] & 4 \cdot [\theta \ \ \varphi]
\end{array}\right]
$$

- which gives:

$$
= \left[\begin{array}{cccc|cc}
\alpha & \beta & 2\alpha & 2\beta & 4\alpha & 4\beta
\\
\hline
\theta & \varphi & 2\theta & 2\varphi & 4\theta & 4\varphi
\end{array}\right]
$$

Hence:

$$
[1 \ \ 2 \ | \ 4] \circ \begin{bmatrix}
\alpha & \beta
\\
\hline
\theta & \varphi
\end{bmatrix}
$$

$$
= \left[\begin{array}{cccc|cc}
\alpha & \beta & 2\alpha & 2\beta & 4\alpha & 4\beta
\\
\hline
\theta & \varphi & 2\theta & 2\varphi & 4\theta & 4\varphi
\end{array}\right]
$$
