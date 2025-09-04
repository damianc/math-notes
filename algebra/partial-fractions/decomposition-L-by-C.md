# Partial Fractions: Decomposition of (px+q) ÷ (x-a)³

## Form of Decomposition

$$
\large
\frac{px+q}{(x-a)^3} = \frac{A}{x-a} + \frac{B}{(x-a)^2} + \frac{C}{(x-a)^3}
$$

## Decomposition

#### 1. By multiplying both sides by the LHS denominator $(x-a)^3$ , we get:

$$
px+q = A(x-a)^2 + B(x-a) + C
$$

#### 2. Apply convenient substitution $x=a$ to obtain $C$:

$$
\begin{array}{l}
pa+q = A(a-a)^2 + B(a-a) + C
\\
{\color{royalblue}C} = {\color{royalblue}pa+q}
\end{array}
$$

#### 3. Apply convenient substitution $x=x_1$ and then $x=x_2$ to obtain a system of equations:

$$
\begin{array}{l}
px+q = A(x_1-a)^2 + B(x_1-a) + C
\\
px+q = A(x_2-a)^2 + B(x_2-a) + C
\end{array}
$$

#### 4. Solve the equations to obtain $A$ and $B$

#### 5. Insert the obtained terms into the partial fractions:

$$
\frac{px+q}{(x-a)^3} = \frac{\color{red}A}{x-a} + \frac{\color{green}B}{(x-a)^2} + \frac{\color{royalblue}C}{(x-a)^3}
$$

## Example

$$
\large
\frac{2x+3}{(x-1)^3} = \frac{A}{x-1} + \frac{B}{(x-1)^2} + \frac{C}{(x-1)^3}
$$

- by multiplying both sides by the LHS denominator $(x-1)^3$, we get:

$$
2x+3 = A(x-1)^2 + B(x-1) + C
$$

- apply convenient substitution $x=1$ to obtain $C$:

$$
\begin{array}{l}
2+3 = A(1-1)^2 + B(1-1) + C
\\
{\color{royalblue}C} = {\color{royalblue}5}
\end{array}
$$

- apply convenient substitution to obtain a system of equations; let $x_1=0$ and $x_2=2$:

$$
\small
\begin{array}{l|l}
0+3=A(0-1)^2+B(0-1)+C & 4+3=A(2-1)^2+B(2-1)+C
\\
3=A-B+C & 7=A+B+C
\\
3=A-B+5 & 7=A+B+5
\\
3-5=A-B & 7-5=A+B
\\
A-B=-2 & A+B=2
\end{array}
$$

$$
\begin{cases}
A-B = -2
\\
A+B = 2
\end{cases}
$$

- solve the equations to obtain $A$ and $B$:

$$
\begin{array}{l}
A-B = -2
\\
A+B = 2
\\
\ 
\\
(A-B)+(A+B) = 0
\\
2A = 0
\\
{\color{red}A} = {\color{red}0}
\\
\ 
\\
0+B = 2
\\
{\color{green}B} = {\color{green}2}
\end{array}
$$

- insert the obtained terms into the partial fractions:

$$
\begin{array}{rl}
\frac{2x+3}{(x-1)^3} & = \frac{\color{red}A}{x-1} + \frac{\color{green}B}{(x-1)^2} + \frac{\color{royalblue}C}{(x-1)^3}
\\
\ 
\\
& = \frac{\color{red}0}{x-1} + \frac{\color{green}2}{(x-1)^2} + \frac{\color{royalblue}5}{(x-1)^3}
\\
\ 
\\
& = \frac{\color{green}2}{(x-1)^2} + \frac{\color{royalblue}5}{(x-1)^3}
\end{array}
$$

