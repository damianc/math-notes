# Cube of a Sum

Most generally:

$$
\left(
\sum_{i=1}^n a_i
\right)^3 =
\sum_{j=1}^n \sum_{k=1}^n \sum_{l=1}^n
a_j a_k a_l
$$

With grouped terms:

$$
\begin{array}{ll}
\displaystyle
\left(\sum_{i=1}^n a_i\right)^3 &
\displaystyle = \left[
\sum_{i=1}^n a_i^3
\right]
\\
\ 
\\
& \displaystyle \quad + \ 6 \left[
\sum_{i=1}^{n-2}
\sum_{j=i+1}^{n-1}
\sum_{k=j+1}^n
a_i a_j a_k
\right]
\\
\ 
\\
& \displaystyle \quad + \ 3 \left[
\sum_{i=1}^n a_i^2 \cdot
\sum_{j=1}^n
a_j (1-\delta_{ij})
\right]
\end{array}
$$

Some first expansions are:

$$
\begin{array}{ll}
(a+b)^3 & = a^3 + b^3
\\
& \quad + \ 3(a^2b + ab^2)
\\
\ 
\\
(a+b+c)^3 & = a^3 + b^3 + c^3
\\
& \quad + \ 6abc
\\
& \quad + \ 3(
\\
& \quad\quad a^2(b+c) \ + 
\\
& \quad\quad b^2(a+c) \ +
\\
& \quad\quad c^2(a+b)
\\
& \quad )
\\
\ 
\\
(a+b+c+d)^3 & = a^3 + b^3 + c^3 + d^3
\\
& \quad + \ 6(abc+abd+acd+bcd)
\\
& \quad + \ 3(
\\
& \quad\quad a^2(b+c+d) \ +
\\
& \quad\quad b^2(a+c+d) \ +
\\
& \quad\quad c^2(a+b+d) \ +
\\
& \quad\quad d^2(a+b+c)
\\
& \quad )
\end{array}
$$

## Negative Summands

The above formulas hold for sums with negative summands, just treat $-x$ like $+(-x)$.

$$
\begin{array}{ll}
(a-b)^3 & = (a+(-b))^3
\\
& = a^3 + (-b)^3 + 3(a^2 \cdot (-b) + a \cdot (-b)^2)
\\
& = a^3 - b^3 + 3(-a^2b + ab^2)
\\
& = a^3 - b^3 + 3(ab^2 - a^2b)
\\
& = a^3 - b^3 + 3ab^2 - 3a^2b
\end{array}
$$
