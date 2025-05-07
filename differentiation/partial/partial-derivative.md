# Partial Derivatives

For a function of several variables, finding the **partial derivative** is performed with respect to one of the variables, hence others are moved before the derivative as they become constants, for example:

$$
\frac{\partial}{\partial x} x^2 {\color{blue} y^2} = {\color{blue} y^2} \left(\frac{\partial}{\partial x} x^2 \right) = 2x{\color{blue} y^2}
$$

## Higher-Order and Mixed Derivatives

A **higher-order derivative** poses **partial derivatives** with respect to the same variable, for example:

$$
\frac{\partial^2 f}{\partial x^2} = \frac{\partial}{\partial x} \left(
\frac{\partial f}{\partial x}
\right)
$$

Such a derivative can be found with respect to different variables. Then it is a **mixed derivative**, for example:

$$
\frac{\partial^2 f}{\partial x \partial y} = \frac{\partial}{\partial x} \left(\frac{\partial f}{\partial y}\right)
$$

### Examples

$$
\begin{array}{rl}
\frac{\partial^2}{\partial x^2} 2x^3 & = \frac{\partial}{\partial x} \left(
\frac{\partial}{\partial x} 2x^3
\right)
\\
\ 
\\
& = \frac{\partial}{\partial x} 6x^2
\\
\ 
\\
& = 12x
\end{array}
$$

$$
\begin{array}{rl}
\frac{\partial^2}{\partial x \partial y} x^2 \sin(y) & = \frac{\partial}{\partial x} \left(
\frac{\partial}{\partial y} x^2 \sin(y)
\right)
\\
\ 
\\
& = \frac{\partial}{\partial x} x^2 \cos(y)
\\
\ 
\\
& = 2x \cos(y)
\end{array}
$$
