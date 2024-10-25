# Integration by Parts

Integration by parts can be performed with use of _UV formula_, or alternatively with _functional formula_.

- _UV formula_:

$$
\int {\color{blue}u}\ {\color{red}dv} = {\color{blue}u}{\color{green}v} - \int {\color{green}v}\ {\color{purple}du}
$$

- alternative _functional formula_:

$$
\int {\color{blue}f(x)}{\color{red}g'(x)} = {\color{blue}f(x)}{\color{green}g(x)} - \int {\color{green}g(x)}{\color{purple}f'(x)}\ dx
$$

where:

- $\color{blue}u$ and $\color{blue}f(x)$ - one of given functions (chosen according to the **ILATE rule** below)
- $\color{red}dv$ and $\color{red}g'(x)$ - the other function
- $\color{purple}du$ and $\color{purple}f'(x)$ - a derivative of $\color{blue}u$ or $\color{blue}f(x)$
- $\color{green}v$ and $\color{green}g(x)$ - an integral of $\color{red}dv$ or $\color{red}g'(x)$

> **ILATE rule**
> 
> The **ILATE rule** (also known as **LIATE**) is used to pick _the first function_ - one denoted by $\color{blue}u$ or $\color{blue}f(x)$. This is a list of function types that enumerates their priority in descending order:
> 
> 1. **I** - inverse trigonometric function
> 2. **L** - logarithmic function
> 3. **A** - algebraic function
> 4. **T** - trigonometric function
> 5. **E** - exponential function
> 
> For example, for a pair of _algebraic_ and _exponential_ functions, the _algebraic_ function is _the first function_, i.e., $\color{blue}u$ or $\color{blue}f(x)$.

## Algorithm

Example integrand: ${\color{blue}x} \cdot {\color{red}e^x}$:

$$
\large
\int\ {\color{blue}x} \cdot {\color{red}e^x}
$$

1. Pick _the first function_ (sticking to the **ILATE rule**) and denote it as $\color{blue}u$:

$$
{\color{blue}u} = x
$$

2. Denote the other function as $\color{red}dv$:

$$
{\color{red}dv} = e^x
$$

3. Get a derivative of $\color{blue}u$ and denote it as $\color{purple}du$:

$$
{\color{purple}du} = {\color{blue}u}' = [x]' = 1
$$

4. Get an integral of $\color{red}dv$ and denote it as $\color{green}v$:

$$
{\color{green}v} = \int {\color{red}dv} = \int e^x\ dx = e^x
$$

5. Replace terms in the formula with respective functions/values:

$$
\int {\color{blue}u}\ {\color{red}dv} = {\color{blue}u}{\color{green}v} - \int {\color{green}v}\ {\color{purple}du}
$$

$$
\int {\color{blue}x} \cdot {\color{red}e^x}\ dx = {\color{blue}x} \cdot {\color{green}e^x} - \int {\color{green}e^x} \cdot {\color{purple}1} \ dx
$$

6. Do remaining math:

$$
\begin{array}{rl}
\int {\color{blue}x} \cdot {\color{red}e^x} \ dx & = {\color{blue}x} \cdot {\color{green}e^x} - \int {\color{green}e^x} \cdot {\color{purple}1} \ dx
\\
& = x \cdot e^x - e^x + C
\\
& = (x-1)e^x + C
\end{array}
$$


