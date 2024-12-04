# Operations on Complex Numbers

The following complex numbers are used in formulas below:

> $z = a + bi$  
> $z_1 = a_1 + b_1 i$  
> $z_2 = a_2 + b_2 i$

## Addition/Subtraction

$$
z_1 \pm z_2 = (a_1 \pm a_2) + (b_1 \pm b_2)i
$$

## Multiplication

$$
\begin{array}{rl}
z_1 z_2 & = {\tiny (a_1+b_1 i)(a_2+b_2 i)}
\\
& = (a_1a_2-b_1b_2)+(a_1b_2+a_2b_1)i
\end{array}
$$

### Multiplication by Scalar

> A scalar $k$ can be perceived as a complex number $k+0i$.

$$
\begin{array}{rl}
kz = {\tiny k(a+bi)} & = {\tiny (k+0i)(a+bi)}
\\
& = ka+kbi
\end{array}
$$

## Division

$$
\begin{array}{rl}
\frac{z_1}{z_2} & = {\tiny \frac{(a_1+b_1 i)(a_2-b_2 i)}{a_2^2+b_2^2}}
\\
\ 
\\
& = \frac{a_1a_2+b_1b_2}{a_2^2+b_2^2} + \frac{b_1a_2-a_1b_2}{a_2^2+b_2^2} i
\end{array}
$$

### Division by Scalar

$$
\begin{array}{rl}
\frac{z}{k} = {\tiny\frac{a+bi}{k}} & = {\tiny \frac{a+bi}{k+0i}}
\\
\ 
\\
& = \frac{a}{k} + \frac{b}{k} i
\end{array}
$$

## Example Calculations

- for $z_1=2+i$ and $z_2=4+3i$:

$$
\begin{array}{l}
z_1 + z_2 = (2+4)+(1+3)i = 6+4i
\\
z_1 - z_2 = (2-4)+(1-3)i = -2-2i
\\
z_2 - z_1 = (4-2)+(3-1)i = 2+2i
\end{array}
$$

$$
\begin{array}{rl}
z_1z_2 & = (2 \cdot 4 - 1 \cdot 3)+(2 \cdot 3 + 1 \cdot 4)i
\\
& = (8-3)+(6+4)i
\\
& = 5+10i
\end{array}
$$

$$
\begin{array}{rl}
\frac{z_1}{z_2} & = \frac{2+i}{4+3i}
\\
\ 
\\
& = \frac{2 \cdot 4 + 1 \cdot 3}{4^2 + 3^2} + \frac{1 \cdot 4 - 2 \cdot 3}{4^2 + 3^2} i
\\
\ 
\\
& = \frac{8+3}{16+9} + \frac{4-6}{16+9} i
\\
\ 
\\
& = \frac{11}{25} + \frac{-2}{25} i = \frac{1}{25} (11-2i)
\end{array}
$$

- for $z=2+3i$ and $k=4$:

$$
kz = 4(2+3i) = 8+12i
$$

- for $z=6+9i$ and $k=3$:

$$
\frac{z}{k} = \frac{6+9i}{3} = \frac{6}{3} + \frac{9}{3} i = 2+3i
$$

$$
\begin{array}{rl}
\frac{k}{z} & = \frac{3}{6+9i} = \frac{3+0i}{6+9i}
\\
\ 
\\
& = \frac{3 \cdot 6 + 0 \cdot 9}{6^2+9^2} + \frac{0 \cdot 6 - 3 \cdot 9}{6^2+9^2} i
\\
\ 
\\
& = \frac{18}{36+81} + \frac{-27}{36+81} i
\\
\ 
\\
& = \frac{18}{117} - \frac{27}{117} i
\\
\ 
\\
& = \frac{2}{13} - \frac{3}{13} i = \frac{1}{13} (2-3i)
\end{array}
$$
