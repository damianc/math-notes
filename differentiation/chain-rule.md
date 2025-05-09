# Chain Rule

$$
\Large
[\ f(g(x))\ ]' = f'(g(x)) \cdot g'(x)
$$


| Step | Example 1 | Example 2 | Example 3 |
|--|--|--|--|
| | $$\frac{d}{dx}\ \sin(x^2)$$ | $$\frac{d}{dx}\ e^{3x}$$ | $$\frac{d}{dx}\ \ln(x^2+4x)$$ |
| **1**.Identify outer function $f(x)$ | $$f(x)=\sin(x)$$ | $$f(x)=e^x$$ | $$f(x)=\ln(x)$$ |
| **2**.Identify inner function $g(x)$ | $$g(x)=x^2$$ | $$g(x)=3x$$ | $$g(x)=x^2+4x$$ |
| **3**.Let $u$ be assigned the inner function $g(x)$ | $$u=g(x)=x^2$$ | $$u=g(x)=3x$$ | $$u=g(x)=x^2+4x$$ |
| **4**.Differentiate the outer function $f(x)$ with respect to $u$ | $$f'(x)=\frac{d}{du} \sin(u)=\cos(u)$$ | $$f'(x)=\frac{d}{du} e^u=e^u$$ | $$f'(x)=\frac{d}{du} \ln(u)=\frac{1}{u}$$ |
| **5**.Differentiate the inner function $g(x)$ with respect to $x$ | $$g'(x)=\frac{d}{dx} x^2=2x$$ | $$g'(x)=\frac{d}{dx} 3x=3$$ | $$g'(x)=\frac{d}{dx} x^2+4x=2x+4$$ |
| **6**.Apply the chain rule | $$f'(g(x))\ g'(x)$$ | $$f'(g(x))\ g'(x)$$ | $$f'(g(x))\ g'(x)$$ |
| | $$\cos(x^2) \cdot 2x$$ | $$e^{3x} \cdot 3$$ | $$\frac{1}{x^2+4x} \cdot (2x+4)$$ |
| **DONE** | $$\frac{d}{dx} \sin(x^2) =$$ | $$\frac{d}{dx} e^{3x} =$$ | $$\frac{d}{dx} \ln(x^2+4x) =$$ |
| | $$2x \cos(x^2)$$ | $$3e^{3x}$$ | $$\frac{2x+4}{x^2+4x} = \frac{2(x+2)}{x(x+4)}$$ |

> As the **Example 3** reads:
> $$\frac{d}{dx} \ln(f(x)) = \frac{f'(x)}{f(x)}$$

> Due to the above:
> $$\int \frac{f'(x)}{f(x)}\ dx = \ln(f(x)) + C$$

## The Chain Rule Partially Defined with Specific Functions

$$
\begin{array}{ll}
\text{\tiny trigonometric}
\\
\ 
\\
\frac{d}{dx} \sin(g(x)) & = \cos(g(x))g'(x)
\\
\ 
\\
\frac{d}{dx} \cos(g(x)) & = -\sin(g(x))g'(x)
\\
\ 
\\
\frac{d}{dx} \tan(g(x)) & = \sec^2(g(x))g'(x)
\\
\ 
\\
\text{\tiny exponential}
\\
\ 
\\
\frac{d}{dx} e^{g(x)} & = e^{g(x)}g'(x)
\\
\ 
\\
\frac{d}{dx} a^{g(x)} & = a^{g(x)} \ln(a) g'(x)
\\
\ 
\\
\text{\tiny logarithmic}
\\
\ 
\\
\frac{d}{dx} \ln(g(x)) & = \frac{g'(x)}{g(x)}
\\
\ 
\\
\frac{d}{dx} \log_b(g(x)) & = \frac{g'(x)}{g(x) \ln(b)}
\\
\ 
\\
\text{\tiny power}
\\
\ 
\\
\frac{d}{dx} g^2(x) & = 2 g(x) g'(x)
\\
\ 
\\
\frac{d}{dx} g^p(x) & = pg^{p-1}(x) g'(x)
\end{array}
$$
