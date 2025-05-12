# Exercise: Find Geometric Sequence by Sums

Find such a geometric sequence that sum of first six terms (**1-6**) is **189**, and sum of next six terms (**7-12**) is **12096**.

$$
\begin{cases}
S_{1-6} = 189
\\
S_{7-12} = 12096
\end{cases}
$$

## Solution

- write formulas for sum of terms:

$$
\begin{array}{lll}
S_{1-6} & = \boldsymbol{a_1 \cdot \frac{1-q^6}{1-q}} & = 189
\\
S_{7-12} & = \boldsymbol{a_1 q^6 \cdot \frac{1-q^6}{1-q}} & = 12096
\end{array}
$$

- evaluate their quotient:

$$
\frac{S_{7-12}}{S_{1-6}} = \frac{12096}{189} = 64
$$

- this time evaluate their quotient with use of the formulas to obtain $q$:

$$
\begin{array}{ll}
\frac{S_{7-12}}{S_{1-6}} = 64 & = \frac{
a_1 q^6 (1-q^6) : (1-q)
}{
a_1 (1-q^6) : (1-q)
}
\\
\ 
\\
& = \frac{a_1 q^6 (1-q^6)}{1-q} \cdot \frac{1-q}{a_1 (1-q^6)}
\\
\ 
\\
& = q^6 \cdot \frac{a_1 (1-q^6)(1-q)}{a_1 (1-q^6)(1-q)}
\\
\ 
\\
& = q^6 \cdot 1 = q^6
\\
\ 
\\
q^6 = 64 & \color{gray}{| \sqrt[6]{\ \ }}
\\
q = 2
\end{array}
$$

- use $q$ to obtain $a_1$ from the first sum:

$$
\begin{array}{l}
189 = a_1 \cdot \frac{1-q^6}{1-q}
\\
\ 
\\
189 = a_1 \cdot \frac{1-2^6}{1-2}
\\
189 = a_1 \cdot \frac{1-64}{1-2}
\\
189 = a_1 \cdot \frac{-63}{-1}
\\
189 = 63 a_1
\\
\ 
\\
a_1 = \frac{189}{63}
\\
\boldsymbol{a_1 = 3}
\end{array}
$$

Hence the solution is:

$$
\begin{array}{l}
q = 2
\\
a_1 = 3
\\
\ 
\\
\\{
3 \cdot 2^{n-1} \in \Bbb{Z} \ | \ n \geqslant 1
\\}
\\
\\{
3,6,12,24,48,96, \dots
\\}
\end{array}
$$
