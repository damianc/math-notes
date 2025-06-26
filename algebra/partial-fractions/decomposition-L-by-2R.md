# Partial Fractions: Decomposition of (px+q) ÷ [(x-a)(x-b)]

## Form of Decomposition

$$
\large
\frac{px+q}{(x-a)(x-b)} = \frac{A}{x-a} + \frac{B}{x-b}
$$

## Decomposition

#### 1. Multiply both sides by the LHS denominator $(x-a)(x-b)$:

$$
\frac{(px+q)(x-a)(x-b)}{(x-a)(x-b)} = \frac{A(x-a)(x-b)}{x-a} + \frac{B(x-a)(x-b)}{x-b}
$$

$$
px+q = A(x-b) + B(x-a)
$$

#### 2. Expand the RHS expression and combine like terms

$$
\begin{array}{rl}
px+q & = Ax-Ab+Bx-Ba
\\
& = (A+B)x-Ab-Ba
\end{array}
$$

#### 3. Match terms on both sides to obtain a system of equations

$$
{\color{blue} p}x+{\color{purple} q} = {\color{blue} (A+B)}x{\color{purple} -Ab-Ba}
$$

$$
\begin{cases}
p = A+B
\\
q = -Ab-Ba
\end{cases}
$$

#### 4. Solve the equations

- getting $A$:

$$
\begin{array}{l}
B = p-A
\\
\ 
\\
q = -Ab-(p-A)a
\\
q = -Ab-[pa-Aa]
\\
q = -Ab-pa+Aa
\\
q+pa = Aa-Ab
\\
q+pa = A(a-b)
\\
\ 
\\
{\color{red} A} = {\color{red} \frac{q+pa}{a-b}}
\end{array}
$$

- getting $B$:

$$
\begin{array}{l}
A = p-B
\\
\ 
\\
q = -(p-B)b-Ba
\\
q = -[pb-Bb]-Ba
\\
q = -pb+Bb-Ba
\\
q+pb = Bb-Ba
\\
q+pb = B(b-a)
\\
\ 
\\
{\color{green} B} = {\color{green} \frac{q+pb}{b-a}}
\end{array}
$$

#### 5. Insert the obtained terms into the partial fractions

$$
\begin{array}{rl}
\frac{px+q}{(x-a)(x-b)} & = \frac{{\color{red} A}}{x-a} + \frac{{\color{green} B}}{x-b}
\\
\ 
\\
& = \frac{{\color{red} ap+q}}{{\color{red} (a-b)}(x-a)} + \frac{{\color{green} pb+q}}{{\color{green} (b-a)}(x-b)}
\end{array}
$$

## Example

$$
\large
\frac{2x+3}{(x-1)(x+2)} = \frac{A}{x-1} + \frac{B}{x+2}
$$

- multiply both sides by the LHS denominator $(x-1)(x+2)$:

$$
\frac{(2x+3)(x-1)(x+2)}{(x-1)(x+2)} = \frac{A(x-1)(x+2)}{x-1} + \frac{B(x-1)(x+2)}{x+2}
$$

$$
2x+3 = A(x+2) + B(x-1)
$$

- expand the RHS expression and combine like terms:

$$
\begin{array}{rl}
2x+3 & = A(x+2)+B(x-1)
\\
& = Ax+2A+Bx-B
\\
& = (A+B)x+2A-B
\end{array}
$$

- match terms on both sides to obtain a system of equations:

$$
{\color{blue} 2}x+{\color{purple} 3} = {\color{blue} (A+B)}x+{\color{purple} 2A-B}
$$

$$
\begin{cases}
2 = A+B
\\
3 = 2A-B
\end{cases}
$$

- solve the equations:

$$
\begin{array}{l|cl}
B=2-A && A=2-B
\\
\ 
\\
3=2A-(2-A) && 3=2(2-B)-B
\\
3=2A-2+A && 3=4-2B-B
\\
5=2A+A && 3=4-3B
\\
5=3A && 1=3B
\\
\ 
\\
{\color{red} A}={\color{red} \frac{5}{3}} && {\color{green} B} = {\color{green} \frac{1}{3}}
\end{array}
$$

- insert the obtained terms into the partial fractions:

$$
\begin{array}{rl}
\frac{2x+3}{(x-1)(x+2)} & = \frac{\color{red} A}{x-1} + \frac{\color{green} B}{x+2}
\\
\ 
\\
& = \frac{\color{red} 5}{{\color{red} 3}(x-1)} + \frac{\color{green} 1}{{\color{green} 3}(x+2)}
\end{array}
$$
