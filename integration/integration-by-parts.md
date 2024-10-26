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

Example integrand: ${\color{blue}x} \cdot {\color{red}e^x}$

$$
\large
\int\ {\color{blue}x} \cdot {\color{red}e^x}
$$

1. Pick _the first function_ (sticking to the **ILATE rule**) and denote it as $\color{blue}u$:

> $x$ is algebraic (**A**) function, $e^x$ is exponential (**E**) function: algebraic function has higher priority as **A** stands before **E** in **LIATE**

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

## Definite Integration by Parts

- _UV formula_:

$$
\int_a^b {\color{blue}u}\ {\color{red}dv} = \Bigl[{\color{blue}u}{\color{green}v}\Bigr]_a^b - \int_a^b {\color{green}v}\ {\color{purple}du}
$$

- _functional formula_:

$$
\int_a^b {\color{blue}f(x)}\ {\color{red}g'(x)}\ dx = \Bigl[{\color{blue}f(x)}{\color{green}g(x)}\Bigr]_a^b - \int_a^b {\color{green}g(x)}\ {\color{purple}f'(x)}\ dx
$$

> $[f(x)]_a^b = f(b)-f(a)$

### Example

Example integrand: ${\color{red}1} \cdot {\color{blue}\ln(x)}$  
Example interval of integration: $\langle 1,e \rangle$

$$
\int_1^e {\color{blue}\ln(x)}\ dx =
\int_1^e {\color{red}1} \cdot {\color{blue}\ln(x)}\ dx
$$

$$
\begin{array}{ll}
{\color{blue}u}=\ln(x) & {\color{purple}du}=\frac{1}{x}
\\
{\color{red}dv}=1 & {\color{green}v}=x
\end{array}
$$

$$
\int_a^b {\color{blue}u}\ {\color{red}dv} = \Bigl[{\color{blue}u}{\color{green}v}\Bigr]_a^b - \int_a^b {\color{green}v}\ {\color{purple}du}
$$

$$
\begin{array}{rl}
\displaystyle\int_1^e {\color{blue}\ln(x)} \cdot {\color{red}1} & = \Bigl[{\color{blue}\ln(x)} \cdot {\color{green}x}\Bigr]_1^e - \displaystyle\int_1^e {\color{green}x} \cdot {\color{purple}\frac{1}{x}}
\\
\ 
\\
& = \Bigl[\ln(x) \cdot x\Bigr]_1^e - \Bigl[x\Bigr]_1^e
\\
\ 
\\
& = \Bigl[\ln(e) \cdot e - \ln(1) \cdot 1\Bigr] - \Bigl[e-1\Bigr]
\\
\ 
\\
& = \Bigl[e-0\Bigr] - \Bigl[e-1\Bigr]
\\
\ 
\\
& = 1
\end{array}
$$

## Apparent Recursion

Sometimes we may end up with apparent recursion when using integration by parts (especially for product of trigonometric functions).

- let's take integrand $\sin(x) \cos(x)$:

$$
\int {\color{blue}\sin(x)}\ {\color{red}\cos(x)}\ dx
$$

$$
\begin{array}{ll}
{\color{blue}u} = \sin(x) & {\color{purple}du} = \cos(x)
\\
{\color{red}dv} = \cos(x) & {\color{green}v} = \sin(x)
\end{array}
$$

$$
\int {\color{blue}u}\ {\color{red}dv} = {\color{blue}u}{\color{green}v} - \int {\color{green}v}\ {\color{purple}du}
$$

$$
\int {\color{blue}\sin(x)}\ {\color{red}\cos(x)}\ dx = {\color{blue}\sin(x)}\ {\color{green}\sin(x)} - \int {\color{green}\sin(x)}\ {\color{purple}\cos(x)}\ dx
$$

- we have the same integral on both sides what apparently leads to infinite recursion:

$$
{\color{#f80}\int \sin(x)\cos(x)\ dx} = \sin^2(x) - {\color{#f80}\int \sin(x)\cos(x)\ dx}
$$

- nonetheless, it's still equation that can be altered - add $\color{#f80}\int \sin(x)\cos(x)$ to both sides:

$$
{\color{#f80}\int \sin(x)\cos(x)\ dx} + {\color{#f80}\int \sin(x) \cos(x)\ dx} = \sin^2(x)
$$

$$
\equiv
$$

$$
2 {\color{#f80}\int \sin(x)\cos(x)\ dx} = \sin^2(x)
$$

- continue transformation, here divide both sides by 2:

$$
{\color{#f80}\int \sin(x)\cos(x)\ dx} = \frac{1}{2} \sin^2(x)
$$

- hence the final integral:

$$
\int \sin(x)\cos(x)\ dx = \frac{1}{2} \sin^2(x) + C
$$


