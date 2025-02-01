# Extracting Variables

## Subtraction

$$
\begin{array}{lcl}
x-a = n & \implies & x = n+a
\\
a-x = n & \implies & x = a-n
\end{array}
$$

## Quotient

$$
\begin{array}{lcl}
\frac{x}{a} = n & \implies & x = na
\\
\ 
\\
\frac{a}{x} = n & \implies & x = \frac{a}{n}
\end{array}
$$

## Power

$$
\begin{array}{lcl}
x^p = n & \implies & x = \sqrt[p]{n}
\\
a^x = n & \implies & x = \log_a(n)
\\
\ 
\\
e^x = n & \implies & x = \ln(n)
\end{array}
$$

## Radical

$$
\begin{array}{lcl}
\sqrt[d]{x} = n & \implies & x = n^d
\\
\sqrt[x]{a} = n & \implies & x = \log_n(a)
\\
\ 
\\
\sqrt[x]{e} = n & \implies & x = \log_n(e) = \frac{1}{\ln(n)}
\end{array}
$$

## Logarithm

$$
\begin{array}{lcl}
\log_b(x) = n & \implies & x = b^n
\\
\log_x(a) = n & \implies & x = \sqrt[n]{a}
\\
\ 
\\
\ln(x) = n & \implies & x = e^n = \exp(n)
\\
\log_x(e) = n & \implies & x = \sqrt[n]{e} = \exp\left(\frac{1}{n}\right)
\end{array}
$$

## Function

> $f^{-1}(\square)$ denotes an inverse function

$$
\begin{array}{lcl}
{\large f(kx) = n} & \implies & {\large x = \frac{1}{k} f^{-1}(n)}
\\
\ 
\\
\sin(kx) = n & \implies & x = \frac{1}{k} \arcsin(n)
\\
\ 
\\
mx+i = n & \implies & x = \frac{n-i}{m}
\\
\ 
\\
\frac{ax+b}{cx+d} = n & \implies & x = \frac{nd-b}{a-nc}
\\
\ 
\\
a(x-z)(x+z) = n & \implies & x = \sqrt{\frac{n}{a} + z^2}
\\
\ 
\\
ax^2+bx+c = n & \implies & x = \sqrt{
 \frac{x-c}{a} + \left(
  \frac{b}{2a}
 \right)^2
} - \frac{b}{2a}
\\
& & \text{or}
\\
& \implies & x = \sqrt{\frac{n-q}{a}} + p
\\
& & \text{where}
\\
& & p = \frac{-b}{2a} \text{ and } q = c-ap^2
\end{array}
$$

## Derivation

- $a^x = n \implies x = \log_a(n)$

$$
\begin{array}{ll}
a^x = n
\\
& \backslash \ln(\square)
\\
\ln(a^x) = \ln(n)
\\
& {\small \because \ln(k^p) = p \ln(k)}
\\
x \ln(a) = \ln(n)
\\
& \backslash : \ln(a)
\\
x = \frac{\ln(n)}{\ln(a)} = \log_a(n)
\end{array}
$$

- $\sqrt[x]{a} = n \implies x = \log_n(a)$

$$
\begin{array}{ll}
\sqrt[x]{a} = n
\\
& \backslash \ln(\square)
\\
\ln(\sqrt[x]{a}) = \ln(n)
\\
& {\small \because \ln(\sqrt[d]{k}) = \frac{\ln(k)}{d} }
\\
\frac{1}{x} \ln(a) = \ln(n)
\\
& \backslash \square^{-1}
\\
\frac{x}{\ln(a)} = \frac{1}{\ln(n)}
\\
& \backslash \cdot \ln(a)
\\
x = \frac{\ln(a)}{\ln(n)} = \log_n(a)
\end{array}
$$

> $\square^{-1}$ can be skipped by use of the fact that $\frac{a}{b} = c \implies \frac{a}{c} = b$

- $\log_b(x) = n \implies x = b^n$

$$
\begin{array}{ll}
\log_b(x) = n
\\
& {\small \because \log_b(a) = k \implies b^k = a }
\\
x = b^n
\end{array}
$$

- $\log_x(a) = n \implies x = \sqrt[n]{a}$

$$
\begin{array}{ll}
\log_x(a) = n
\\
& {\small \because \log_b(a) = k \implies b^k = a }
\\
x^n = a
\\
& \backslash \sqrt[n]{\square}
\\
x = \sqrt[n]{a}
\end{array}
$$

- $\frac{ax+b}{cx+d} = n \implies x = \frac{nd-b}{a-nc}$

$$
\begin{array}{ll}
\frac{ax+b}{cx+d} = n
\\
& \backslash \cdot (cx+d)
\\
ax+b = n(cx+d)
\\
& {\small \because k(a+b) = ka+kb}
\\
ax+b = ncx+nd
\\
& \backslash -(ncx+nd)
\\
ax+b-ncx-nd = 0
\\
& \backslash +nd-b
\\
ax-ncx = nd-b
\\
& {\small \because ka+kb = k(a+b)}
\\
x(a-nc) = nd-b
\\
& \backslash : (a-nc)
\\
x = \frac{nd-b}{a-nc}
\end{array}
$$

- $a(x-z)(x+z) = n \implies x = \sqrt{\frac{n}{a}+z^2}$

$$
\begin{array}{ll}
a(x-z)(x+z) = n
\\
& {\small \because (a-b)(a+b) = a^2-b^2}
\\
a(x^2-z^2) = n
\\
& \backslash : a
\\
x^2-z^2 = \frac{n}{a}
\\
& \backslash +z^2
\\
x^2 = \frac{n}{a}+z^2
\\
& \backslash \sqrt{\square}
\\
x = \sqrt{\frac{n}{a}+z^2}
\end{array}
$$

- $ax^2+bx+c=n \implies x=\sqrt{\frac{n-q}{a}}+p$

> conversion from standard form $ax^2+bx+c$ to vertex form $a(x-p)^2+q$ takes place (details)

$$
\begin{array}{ll}
a(x-p)^2+q = n
\\
& \backslash -q
\\
a(x-p)^2 = n-q
\\
& \backslash :a
\\
(x-p)^2 = \frac{n-q}{a}
\\
& \backslash \sqrt{\square}
\\
x-p = \sqrt{\frac{n-q}{a}}
\\
& \backslash +p
\\
x = \sqrt{\frac{n-q}{a}}+p
\end{array}
$$
