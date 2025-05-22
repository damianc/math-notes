# Partial Fractions: Decomposition of (px+q) ÷ [(x-a)(x-b)]

## Form of Decomposition

$$
\large
\frac{px+q}{(x-a)(x-b)} = \frac{A}{x-a} + \frac{B}{x-b}
$$

## Decomposition

#### 1. Sum up the RHS fractions to obtain a common denominator

$$
\frac{px+q}{(x-a)(x-b)} = \frac{A(x-b) + B(x-a)}{(x-a)(x-b)}
$$

#### 2. Compare the numerators of both fractions

$$
px+q = A(x-b)+B(x-a)
$$

- expand the RHS expression

$$
px+q = Ax-Ab+Bx-Ba
$$

- combine like terms of the RHS expression

$$
px+q = (A+B)x-Ab-Ba
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
A = \frac{q+pa}{a-b}
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
B = \frac{q+pb}{b-a}
\end{array}
$$
