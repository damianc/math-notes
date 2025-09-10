# Partial Fractions: Getting the Intercept Form of a Quadratic Denominator

This note shows how to perform conversion of a quadratic denominator to the **intercept form**:

- from the **vertex form**:

$$
\small
\frac{mx+i}{a(x-p)^2+q} \mapsto \frac{mx+i}{a(x-x_1)(x-x_2)}
$$

- from the **standard form**:

$$
\small
\frac{mx+i}{ax^2+bx+c} \mapsto \frac{mx+i}{a(x-x_1)(x-x_2)}
$$

## From the Vertex Form

> $a(x-p)^2+q \ \mapsto \ a(x-x_1)(x-x_2)$

1. First, convert the expression to the **standard form**:

$$
\begin{array}{l}
a(x-p)^2+q \ \mapsto \ ax^2+bx+c
\\
\ 
\\
\begin{cases}
a = a
\\
b = -2ap
\\
c = ap^2+q
\end{cases}
\end{array}
$$

2. Then convert it to the **intercept form** just like below.

> 💡 **DIRECT VERTEX → INTERCEPT CONVERSION**
>
> $x_{1,2} = p \pm \frac{\sqrt{\Delta}}{2a}, \quad \Delta = -4aq$
>
> of course, it's necessary that $\Delta \geq 0$, or - in this case: $\text{sign}(a) \neq \text{sign}(q)$

## From the Standard Form

> $ax^2+bx+c \ \mapsto \ a(x-x_1)(x-x_2)$ or $a(x-x_0)^2$

$$
\begin{array}{l}
\Delta = b^2-4ac
\\
\ 
\\
\begin{cases}
\text{if } \Delta \gt 0: & x_{1,2} = \frac{-b \pm \sqrt{\Delta}}{2a}
\\
\text{if } \Delta = 0: & x_0 = \frac{-b}{2a}
\end{cases}
\end{array}
$$

