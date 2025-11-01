# Obtaining a Random Value

> It applies to JavaScript where `Math.random()` $\in$ [0,1).
>
> Below, let $\tt{R}$ be assigned a value from `Math.random()`.

- value $\in$ [a,b):

$$
{\tt{R}} \cdot (b-a) + a
$$

- value $\in \Bbb{Z} \ \cap$ [a,b):

$$
\begin{array}{l}
\lfloor
{\tt{R}} \cdot (B-A) + A\rfloor
\\
\ 
\\
\text{where: } A = \lceil a \rceil, B = \lfloor b \rfloor
\end{array}
$$

- value $\in \Bbb{Z} \ \cap$ [a,b]:

$$
\begin{array}{l}
\lfloor
{\tt{R}} \cdot (B-A+1) + A\rfloor
\\
\ 
\\
\text{where: } A = \lceil a \rceil, B = \lfloor b \rfloor
\end{array}
$$
