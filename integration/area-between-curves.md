# Area Between Curves

The idea of obtaining the area between curves comes down to subtracting the area of one region from the area of the other region on the interval determined by the common points of the curves.

If there are two curves - $f(x)$ and $g(x)$, and they intersect at $x_1$ and $x_2$, the area $A$ between them is:

$$
A = \int_{x_1}^{x_2} \bigl(g(x) - f(x)\bigr) \ dx
$$

Of course, _minuend_ and _subtrahend_ are chosen so that it makes sense.

## Example

There are two curves:

$$
\begin{array}{l}
f(x) = 4-x
\\
g(x) = 6-x^2
\end{array}
$$

- common points:

$$
\begin{array}{l}
f(x) = g(x)
\\
4-x = 6-x^2
\\
4-x-6+x^2
\\
x^2-x-2
\\
\ 
\\
a = 1
\\
b = -1
\\
c = -2
\\
\ 
\\
\Delta = b^2-4ac = 1+8 = 9
\\
x_{1,2} = \frac{-b \ \mp \ \sqrt{\Delta}}{2a}
\\
\ 
\\
x_1 = \frac{1-\sqrt{9}}{2} = -1
\\
x_2 = \frac{1+\sqrt{9}}{2} = 2
\end{array}
$$

- integrals:

$$
\begin{array}{ll}
I_1 = \displaystyle\int_{x_1}^{x_2} g(x) \ dx & = \displaystyle\int_{-1}^2 (6-x^2) \ dx
\\
& = \left[
6x - \frac{1}{3}x^3
\right]_{-1}^2
\\
& = 15
\\
\ 
\\
I_2 = \displaystyle\int_{x_1}^{x_2} f(x) \ dx & = \displaystyle\int_{-1}^2 (4-x) \ dx
\\
& = \left[
4x - \frac{1}{2}x^2
\right]_{-1}^2
\\
& = 10.5
\end{array}
$$

- the area between curves:

$$
A = I_1 - I_2 = 15-10.5 = 4.5
$$
