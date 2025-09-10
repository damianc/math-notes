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

> For detailed conversion, see [Forms of Quadratic Functions](https://github.com/damianc/math-notes/blob/master/functions/quadratic/forms.md).

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

## Examples

### Example #1: Vertex → Intercept

$$
\begin{array}{l}
{\color{gray} a(x-p)^2+q = \ }
2\left( x+\frac{1}{2} \right)^2 - 12.5
\\
{\small \quad a=2}
\\
{\small \quad p=-\frac{1}{2}}
\\
{\small \quad q=-12.5}
\\
\ 
\\
\Delta = -4aq = -4 \cdot 2 \cdot (-12.5) = 100
\\
\sqrt{\Delta} = 10
\\
\ 
\\
x_1 = p+\frac{\sqrt{\Delta}}{2a} = -\frac{1}{2} + \frac{10}{4} = \frac{5}{2} - \frac{1}{2} = 2
\\
x_2 = p-\frac{\sqrt{\Delta}}{2a} = -\frac{1}{2} - \frac{10}{4} = -\left(\frac{1}{2} + \frac{5}{2}\right) = -3
\\
\ 
\\
{\color{gray} a(x-x_1)(x-x_2) = \ } 2(x-2)(x+3)
\end{array}
$$

> $2\left(x+\frac{1}{2}\right)^2-12.5 \ \equiv \ 2(x-2)(x+3)$

### Example #2: Vertex → Standard → Intercept

1. First **vertex → standard**:

$$
\begin{array}{l}
{\color{gray} a(x-p)^2+q = \ }
2\left( x+\frac{1}{2} \right)^2 - 12.5
\\
{\small \quad a=2}
\\
{\small \quad p=-\frac{1}{2}}
\\
{\small \quad q=-12.5}
\\
\ 
\\
a = 2
\\
b = -2ap = -2 \cdot 2 \cdot \left(-\frac{1}{2}\right) = 2
\\
c = ap^2+q = 2 \cdot \left(-\frac{1}{2}\right)^2 - 12.5 = -12
\\
\ 
\\
{\color{gray} ax^2+bx+c = \ } 2x^2+2x-12
\end{array}
$$

2. Then **standard → intercept**: just like below.

### Example #3: Standard → Intercept

$$
\begin{array}{l}
{\color{gray} ax^2+bx+c = \ }
2x^2+2x-12
\\
{\small \quad a=2}
\\
{\small \quad b=2}
\\
{\small \quad c=-12}
\\
\ 
\\
\Delta = b^2-4ac = 4+96 = 100
\\
\sqrt{\Delta} = 10
\\
\ 
\\
x_1 = \frac{-b+\sqrt{\Delta}}{2a} = \frac{-2+10}{4} = 2
\\
x_2 = \frac{-b-\sqrt{\Delta}}{2a} = \frac{-2-10}{4} = -3
\\
\ 
\\
{\color{gray} a(x-x_1)(x-x_2) = \ } 2(x-2)(x+3)
\end{array}
$$

> $2x^2+2x-12 \ \equiv \ 2(x-2)(x+3)$



