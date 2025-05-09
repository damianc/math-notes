# Operations on Matrices

## Addition/Subtraction

For matrix $C=A \pm B$, its element $c_{ij}$ is a sum/difference of respective elements, that is:

$$
\large
c_{ij} = a_{ij} \pm b_{ij}
$$

For example:

$$
\begin{bmatrix}
{\color{red}a_{11}} & {\color{green}a_{12}}
\\
{\color{blue}a_{21}} & {\color{purple}a_{22}}
\end{bmatrix} \pm \begin{bmatrix}
{\color{red}b_{11}} & {\color{green}b_{12}}
\\
{\color{blue}b_{21}} & {\color{purple}b_{22}}
\end{bmatrix} = \begin{bmatrix}
{\color{red}a_{11} \pm b_{11}} & {\color{green}a_{12} \pm b_{12}}
\\
{\color{blue}a_{21} \pm b_{21}} & {\color{purple}a_{22} \pm b_{22}}
\end{bmatrix}
$$

$$
\begin{bmatrix}
{\color{red}A} & {\color{green}B}
\\
{\color{blue}C} & {\color{purple}D}
\end{bmatrix} \pm \begin{bmatrix}
{\color{red}E} & {\color{green}F}
\\
{\color{blue}G} & {\color{purple}H}
\end{bmatrix} = \begin{bmatrix}
{\color{red}A \pm E} & {\color{green}B \pm F}
\\
{\color{blue}C \pm G} & {\color{purple}D \pm H}
\end{bmatrix}
$$

## Multiplication with Scalar

For matrix $B=k \cdot A$, its element $b_{ij}$ is element $a_{ij}$ multiplied by $k$, that is:

$$
\large
b_{ij} = k \cdot a_{ij}
$$

For example:

$$
{\color{orange}k} \cdot \begin{bmatrix}
a_{11} & a_{12}
\\
a_{21} & a_{22}
\end{bmatrix} = \begin{bmatrix}
{\color{orange}k}a_{11} & {\color{orange}k}a_{12}
\\
{\color{orange}k}a_{21} & {\color{orange}k}a_{22}
\end{bmatrix}
$$

## Multiplication of Matrices

> Details are on the page: [Matrix Multiplication](https://github.com/damianc/math-notes/blob/master/matrices/matrix-multiplication.md)

Having the following function:

$$
\lambda\binom{R}{C} = R_1C_1 + R_2C_2 + \cdots + R_nC_n
$$

Multiplication of matrices $A$ and $B$ can be represented as follows:

$$
A_{m \times n} \cdot B_{n \times p} = \begin{bmatrix}
\lambda\binom{\text{A row }1}{\text{B col }1}
&
\lambda\binom{\text{A row }1}{\text{B col }2}
&
\cdots
&
\lambda\binom{\text{A row }1}{\text{B col }p}
\\
\ 
\\
\lambda\binom{\text{A row }2}{\text{B col }1}
&
\lambda\binom{\text{A row }2}{\text{B col }2}
&
\cdots
&
\lambda\binom{\text{A row }2}{\text{B col }p}
\\
\ 
\\
\vdots & \vdots & \ddots & \vdots
\\
\ 
\\
\lambda\binom{\text{A row }m}{\text{B col }1}
&
\lambda\binom{\text{A row }m}{\text{B col }2}
&
\cdots
&
\lambda\binom{\text{A row }m}{\text{B col }p}
\end{bmatrix}_{m \times p}
$$

For example:

$$
\overbrace{
\begin{bmatrix}
{\color{red}1} & {\color{red}2} & {\color{red}3}
\\
{\color{blue}3} & {\color{blue}4} & {\color{blue}5}
\end{bmatrix}}^{\text{A}} \cdot \overbrace{\begin{bmatrix}{\color{green}2} & {\color{purple}4}
\\
{\color{green}3} & {\color{purple}1}
\\
{\color{green}4} & {\color{purple}2}
\end{bmatrix}}^{\text{B}} =
$$

$$
\begin{bmatrix}
\lambda\binom{
\overbrace{\color{red}1,2,3}^{\text{A row 1}}
}{
\underbrace{\color{green}2,3,4}\_{\text{B col 1}}
}
&
\lambda\binom{
\overbrace{\color{red}1,2,3}^{\text{A row 1}}
}{
\underbrace{\color{purple}4,1,2}\_{\text{B col 2}}
}
\\
\ 
\\
\lambda\binom{
\overbrace{\color{blue}3,4,5}^{\text{A row 2}}
}{
\underbrace{\color{green}2,3,4}\_{\text{B col 1}}
}
&
\lambda\binom{
\overbrace{\color{blue}3,4,5}^{\text{A row 2}}
}{
\underbrace{\color{purple}4,1,2}\_{\text{B col 2}}
}
\end{bmatrix} =
$$

$$
\begin{bmatrix}
{\color{red}1}\cdot{\color{green}2}+{\color{red}2}\cdot{\color{green}3}+{\color{red}3}\cdot{\color{green}4}
&
{\color{red}1}\cdot{\color{purple}4}+{\color{red}2}\cdot{\color{purple}1}+{\color{red}3}\cdot{\color{purple}2}
\\
\ 
\\
{\color{blue}3}\cdot{\color{green}2}+{\color{blue}4}\cdot{\color{green}3}+{\color{blue}5}\cdot{\color{green}4}
&
{\color{blue}3}\cdot{\color{purple}4}+{\color{blue}4}\cdot{\color{purple}1}+{\color{blue}5}\cdot{\color{purple}2}
\end{bmatrix} =
$$

$$
\begin{bmatrix}
20 & 12
\\
38 & 26
\end{bmatrix}
$$

