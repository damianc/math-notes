# Partial Fractions: Decomposition of (px+q) ÷ [(x-a)(x-b)(x-c)]

## Form of Decomposition

$$
\large
\frac{px+q}{(x-a)(x-b)(x-c)} = \frac{A}{x-a} + \frac{B}{x-b} + \frac{C}{x-c}
$$

## Decomposition

#### 1. By multiplying both sides by the LHS denominator $(x-a)(x-b)(x-c)$, we get:

$$
px+q = A(x-b)(x-c) + B(x-a)(x-c) + C(x-a)(x-b)
$$

#### 2. Apply convenient substitution to obtain $A$, $B$ and $C$:

- $x=a$:

$$
\begin{array}{l}
pa+q = A(a-b)(a-c) + B(a-a)(a-c) + C(a-a)(a-b)
\\
pa+q = A(a-b)(a-c)
\\
\ 
\\
{\color{red}A} = {\color{red}\frac{pa+q}{(a-b)(a-c)}}
\end{array}
$$

- $x=b$:

$$
\begin{array}{l}
pb+q = A(b-b)(b-c) + B(b-a)(b-c) + C(b-a)(b-b)
\\
pb+q = B(b-a)(b-c)
\\
\ 
\\
{\color{green}B} = {\color{green}\frac{pb+q}{(b-a)(b-c)}}
\end{array}
$$

- $x=c$:

$$
\begin{array}{l}
pc+q = A(c-b)(c-c) + B(c-a)(c-c) + C(c-a)(c-b)
\\
pc+q = C(c-a)(c-b)
\\
\ 
\\
{\color{royalblue}C} = {\color{royalblue}\frac{pc+q}{(c-a)(c-b)}}
\end{array}
$$

#### 3. Insert the obtained terms into the partial fractions:

$$
\begin{array}{rl}
\frac{px+q}{(x-a)(x-b)(x-c)} & = \frac{\color{red}A}{x-a} + \frac{\color{green}B}{x-b} + \frac{\color{royalblue}C}{x-c}
\\
\ 
\\
& = \frac{\color{red}pa+q}{{\color{red}(a-b)(a-c)}(x-a)} +  \frac{\color{green}pb+q}{{\color{green}(b-a)(b-c)}(x-b)} +  \frac{\color{royalblue}pc+q}{{\color{royalblue}(c-a)(c-b)}(x-c)}
\end{array}
$$

## Example

$$
\large
\frac{2x+3}{(x-1)(x+2)(x-4)} = \frac{A}{x-1} + \frac{B}{x+2} + \frac{C}{x-4}
$$

- by multiplying both sides by the LHS denominator $(x-1)(x+2)(x-4)$, we get:

$$
2x+3 = A(x+2)(x-4) + B(x-1)(x-4) + C(x-1)(x+2)
$$

- apply convenient substitution $x=1$ to obtain $A$:

$$
\begin{array}{l}
2+3 = A(1+2)(1-4) + B(1-1)(1-4) + C(1-1)(1+2)
\\
5 = -9A
\\
\ 
\\
{\color{red}A} = {\color{red}-\frac{5}{9}}
\end{array}
$$

- apply convenient substitution $x=-2$ to obtain $B$:

$$
\begin{array}{l}
-4+3 = A(-2+2)(-2-4) + B(-2-1)(-2-4) + C(-2-1)(-2+2)
\\
-1 = 18B
\\
\ 
\\
{\color{green}B} = {\color{green}-\frac{1}{18}}
\end{array}
$$

- apply convenient substitution $x=4$ to obtain $C$:

$$
\begin{array}{l}
8+3 = A(4+2)(4-4) + B(4-1)(4-4) + C(4-1)(4+2)
\\
11 = 18C
\\
\ 
\\
{\color{royalblue}C} = {\color{royalblue}\frac{11}{18}}
\end{array}
$$

- insert the obtained terms into the partial fractions:

$$
\begin{array}{rl}
\frac{2x+3}{(x-1)(x+2)(x-4)} & = \frac{\color{red}A}{x-1} + \frac{\color{green}B}{x+2} + \frac{\color{royalblue}C}{x-4}
\\
\ 
\\
& = {\color{red}-}\frac{\color{red}5}{{\color{red}9}(x-1)} {\color{green}-}\frac{\color{green}1}{{\color{green}18}(x+2)} + \frac{\color{royalblue}11}{{\color{royalblue}18}(x-4)}
\\
\ 
\\
& = \frac{1}{18}\left(
\frac{\color{royalblue}11}{x-4} {\color{green}-} \frac{\color{green}1}{x+2} {\color{red}-} \frac{\color{red}10}{x-1}
\right)
\end{array}
$$

