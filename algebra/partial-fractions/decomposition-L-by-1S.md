# Partial Fractions: Decomposition of (px+q)÷(x-a)²

## Form of Decomposition

$$
\large
\frac{px+q}{(x-a)^2} = \frac{A}{x-a} + \frac{B}{(x-a)^2}
$$

## Decomposition

#### 1. Multiply both sides by the LHS denominator $(x-a)^2$

$$
\frac{(px+q)(x-a)^2}{(x-a)^2} = \frac{A(x-a)^2}{x-a} + \frac{B(x-a)^2}{(x-a)^2}
$$

$$
px+q = A(x-a) + B
$$

#### 2. Expand the RHS expression

$$
px + q = Ax-Aa+B
$$

#### 3. Match terms on both sides to obtain a system of equations

$$
{\color{royalblue}p}x+{\color{purple}q} = {\color{royalblue}A}x+{\color{purple}B-Aa}
$$

$$
\begin{cases}
p = A
\\
q = B-Aa
\end{cases}
$$

#### 4. Solve the equations

$$
\begin{array}{l}
{\color{red}A} = {\color{red}p}
\\
\ 
\\
q = B-pa
\\
q+pa = B
\\
\ 
\\
{\color{green}B} = {\color{green}q+pa}
\end{array}
$$

#### 5. Insert the obtained terms into the partial fractions

$$
\begin{array}{rl}
\frac{px+q}{(x-a)^2} & = \frac{\color{red}A}{x-a} + \frac{\color{green}B}{(x-a)^2}
\\
\ 
\\
& = \frac{\color{red}p}{x-a} + \frac{\color{green}ap+q}{(x-a)^2}
\end{array}
$$

## Example

$$
\large
\frac{2x+3}{(x-1)^2} = \frac{A}{x-1} + \frac{B}{(x-1)^2}
$$

- multiply both sides by the LHS denominator $(x-1)^2$:

$$
\frac{(2x+3)(x-1)^2}{(x-1)^2} = \frac{A(x-1)^2}{x-1} + \frac{B(x-1)^2}{(x-1)^2}
$$

$$
2x+3 = A(x-1)+B
$$

- expand the RHS expression:

$$
2x+3 = Ax-A+B
$$

- match terms on both sides to obtain a system of equations:

$$
{\color{royalblue}2}x+{\color{purple}3} = {\color{royalblue}A}x+{\color{purple}B-A}
$$

$$
\begin{cases}
2 = A
\\
3 = B-A
\end{cases}
$$

- solve the equations:

$$
\begin{array}{l}
{\color{red}A} = {\color{red}2}
\\
\ 
\\
3 = B-2
\\
B = 3+2
\\
\ 
\\
{\color{green}B} = {\color{green}5}
\end{array}
$$

- insert the obtained terms into the partial fractions:

$$
\begin{array}{rl}
\frac{2x+3}{(x-1)^2} & = \frac{\color{red}A}{x-1} + \frac{\color{green}B}{(x-1)^2}
\\
\ 
\\
& = \frac{\color{red}2}{x-1} + \frac{\color{green}5}{(x-1)^2}
\end{array}
$$


