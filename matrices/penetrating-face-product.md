# Penetrating Face Product

The **penetrating face product** of a matrix $A_{p \times g}$ and a matrix $B$ that consists of $p \times g$ blocks produces a matrix that consists of $p \times g$ blocks such that n-th block is the **Hadamard product** of $A$ and n-th block of $B$.

$$
A [\circ] B = \bigl[
A \circ B_1 \ | \ 
A \circ B_2 \ | \ 
\cdots \ | \ 
A \circ B_n
\bigr]
$$

> You can think about the **penetrating face product** like the **Hadamard product** where a matrix $A$ is repeated to match size of a matrix $B$.

> the **penetrating face product** can be denoted with $[\circ]$ or $\boxed{\bullet}$

## Example

If matrices $A$ and $B$ are as follows:

$$
A = \begin{bmatrix}
1 & 2
\\
3 & 4
\end{bmatrix}
$$

$$
B = \bigl[ B_1 \ | \ B_2 \ | \ B_3 \bigr] = \left[\begin{array}{cc|cc|cc}
\alpha & \beta & \theta & \varphi & \sigma & \pi
\\
\gamma & \delta & \lambda & \mu & \chi & \omega
\end{array}\right]
$$

Then:

$$
A [\circ] B = \bigl[
A \circ B_1 \ | \ 
A \circ B_2 \ | \ 
A \circ B_3
\bigr]
$$

$$
= \left[\begin{array}{cc|cc|cc}
\alpha & 2\beta & \theta & 2\varphi & \sigma & 2\pi
\\
3\gamma & 4\delta & 3\lambda & 4\mu & 3\chi & 4\omega
\end{array}\right]
$$
