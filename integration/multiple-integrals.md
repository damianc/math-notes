# Multiple Integrals

Simply put: begin with innermost integral and go towards outermost integral.


$$
\overbrace{
  {\color{green} \int_0^1}
  \int_2^3
  \underbrace{
    {\color{red} \int_4^5}
    \quad xyz \quad
    {\color{red}dz}
  }_{\color{red}\text{innermost}}
  \ dy \ 
  {\color{green}dx}
}^{
  {\color{green}\text{outermost}}
}
$$

## Integration Process

1. Identify integrals:

$$
{\color{green}\int_0^1}
\int_2^3
{\color{red}\int_4^5}
\quad xyz \quad
{\color{red}dz}\ dy\ {\color{green}dx}
$$

2. Integrate the innermost integral:

$$
\begin{array}{cl}
\displaystyle\int_4^5 xyz\ dz
& = xy \displaystyle\int_4^5 z\ dz
\\
\ 
\\
& = xy\ \Bigl[\frac{z^2}{2}\Bigr]_4^5
\\
\ 
\\
& = xy\ (12.5-8)
\\
& = 4.5xy
\end{array}
$$

> when integrating with respect to the $z$ variable, other variables become constants and thus go before the integral
> (the same applies to any variable an integration is performed with respect to)

3. Integrate another integral:

$$
\begin{array}{cl}
\displaystyle\int_2^3 4.5xy \ dy & =
4.5x \displaystyle\int_2^3 y\ dy
\\
\ 
\\
& = 4.5x \Bigl[\frac{y^2}{2}\Bigr]_2^3
\\
\ 
\\
& = 4.5x(4.5-2)
\\
& = 11.25x
\end{array}
$$

4. Integrate the outermost integral:

$$
\begin{array}{cl}
\displaystyle\int_0^1 11.25x \ dx & =
11.25 \displaystyle\int_0^1 x \ dx
\\
\ 
\\
& = 11.25 \Bigl[\frac{x^2}{2}\Bigr]_0^1
\\
\ 
\\
& = 11.25(0.5-0)
\\
\ 
\\
& = {\large {\color{#2ae} 5.625}}
\end{array}
$$

The obtained value is the result of the integration.
