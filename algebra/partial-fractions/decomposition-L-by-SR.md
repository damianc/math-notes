# Partial Fractions: Decomposition of (px+q) ÷ [(x-a)²(x-c)]

## Form of Decomposition

$$
\large
\frac{px+q}{(x-a)^2 (x-c)} = \frac{A}{x-a} + \frac{B}{(x-a)^2} + \frac{C}{x-c}
$$

## Decomposition

#### 1. By multiplying both sides by the LHS denominator $(x-a)^2 (x-c)$, we get:

$$
px+q = A(x-a)(x-c) + B(x-c) + C(x-a)^2
$$

#### 2. Apply convenient substitution to obtain $A$, $B$ and $C$:

- $x=a$:

$$
\begin{array}{l}
pa+q = A(a-a)(a-c) + B(a-c) + C(a-a)^2
\\
pa+q = B(a-c)
\\
\ 
\\
{\color{green}B} = {\color{green}\frac{pa+q}{a-c}}
\end{array}
$$

- $x=c$:

$$
\begin{array}{l}
pc+q = A(c-a)(c-c) + B(c-c) + C(c-a)^2
\\
pc+q = C(c-a)^2
\\
\ 
\\
{\color{royalblue}C} = {\color{royalblue}\frac{pc+q}{(c-a)^2}}
\end{array}
$$

- $B$ and $C$ are already known, to obtain $A$ let $x$ be assigned any value, for example $x=0$:

$$
\begin{array}{l}
0+q = A(-a)(-c) + B(-c) + C(-a)^2
\\
q = Aac-Bc+Ca^2
\\
q+Bc-Ca^2 = Aac
\\
\ 
\\
{\color{red}A} = {\color{red}\frac{q+Bc-Ca^2}{ac}}
\end{array}
$$

#### 3. Insert the obtained terms into the partial fractions:

$$
\begin{array}{rl}
\frac{px+q}{(x-a)^2 (x-c)} & = \frac{\color{red}A}{x-a} + \frac{\color{green}B}{(x-a)^2} + \frac{\color{royalblue}C}{x-c}
\\
\ 
\\
& = \frac{\color{red}q+Bc-Ca^2}{{\color{red}ac}(x-a)} + \frac{\color{green}pa+q}{{\color{green}(a-c)}(x-a)^2} + \frac{\color{royalblue}pc+q}{{\color{royalblue}(c-a)^2} (x-c)}
\end{array}
$$

## Example

$$
\large
\frac{2x+3}{(x-1)^2 (x-4)} = \frac{A}{x-1} + \frac{B}{(x-1)^2} + \frac{C}{x-4}
$$

- by multiplying both sides by the LHS denominator $(x-1)^2 (x-4)$, we get:

$$
2x+3 = A(x-1)(x-4) + B(x-4) + C(x-1)^2
$$

- apply convenient substitution $x=1$ to obtain $B$:

$$
\begin{array}{l}
2+3 = A(1-1)(1-4) + B(1-4) + C(1-1)^2
\\
5 = -3B
\\
\ 
\\
{\color{green}B} = {\color{green}-\frac{5}{3}}
\end{array}
$$

- apply convenient substitution $x=4$ to obtain $C$:

$$
\begin{array}{l}
8+3 = A(4-1)(4-4) + B(4-4) + C(4-1)^2
\\
11 = 9C
\\
\ 
\\
{\color{royalblue}C} = {\color{royalblue}\frac{11}{9}}
\end{array}
$$

- apply convenient substitution $x=0$ to obtain $A$:

$$
\begin{array}{l}
0+3 = A(-1)(-4) + B(-4) + C(-1)^2
\\
3 = 4A-4B+C
\\
3+4B-C = 4A
\\
\ 
\\
{\color{red}A} = {\color{red}\frac{3+4B-C}{4}} = {\color{red}-\frac{11}{9}}
\end{array}
$$

- insert the obtained terms into the partial fractions:

$$
\begin{array}{rl}
\frac{2x+3}{(x-1)^2 (x-4)} & = \frac{\color{red}A}{x-1} + \frac{\color{green}B}{(x-1)^2} + \frac{\color{royalblue}C}{x-4}
\\
\ 
\\
& = {\color{red}-}\frac{\color{red}11}{{\color{red}9}(x-1)} {\color{green}-}\frac{\color{green}5}{{\color{green}3}(x-1)^2} + \frac{\color{royalblue}11}{{\color{royalblue}9}(x-4)}
\\
\ 
\\
& = \frac{11}{9}\left(
\frac{\color{royalblue}1}{x-4} {\color{red}-}\frac{\color{red}1}{x-1}
\right) {\color{green}-}\frac{\color{green}5}{{\color{green}3}(x-1)^2}
\end{array}
$$



