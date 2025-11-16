# Substitution When There Are Multiple $x$'s

If an integrand consists of multiple expressions that contain $x$, each should be respectively changed.

$$
\begin{array}{ll}
\text{HAVING:}
\\
& \displaystyle u=\sqrt{x}
\\
\ 
\\
{\color{red}\text{WRONG:}}
\\
& \displaystyle \frac{\sqrt{x}-1}{x} \rightarrow \frac{u-1}{x}
\\
\ 
\\
{\color{green}\text{CORRECT:}}
\\
& \displaystyle \frac{\sqrt{x}-1}{x} \rightarrow \frac{u-1}{u^2}
\end{array}
$$

## Detailed Guide

> This very guide covers substitution $dx=[f^{-1}(t)]' \ dt$ rather than just $dx=du/f'(x)$, i.e., an inverse function of an expression is involved 

| | $$\int \frac{\sqrt{x}-1}{x} \ dx$$ | $$\int \frac{e^x}{1+e^x} \ dx$$ | $$\int \frac{\ln(x)}{x} \ dx$$ |
|--|--|--|--|
| 1. Let $t$ be assigned an expression (i.e., $t=f(x)$ ) | $t = \sqrt{x}$ | $t=e^x$ | $t=\ln(x)$ |
| 2. Transform the equation to only obtain $x$ (i.e., $x=f^{-1}(t)$ ) | $x = t^2$ | $x = \ln(t)$ | $x = e^t$ |
| 3. Let $dx$ be assigned a derivative of the above function and $dt$ (i.e., $dx = [f^{-1}(t)]' dt$ ) | $dx = 2t \ dt$ | $dx = \frac{1}{t} dt$ | $dx = e^t dt$ |
| 4. Rewrite integral in terms of $t$ and multiplied by the resultant $dx$ | $$\int \frac{t-1}{t^2} \ 2t \ dt$$ | $$\int \frac{t}{1+t} \cdot \frac{1}{t} \ dt$$ | $$\int \frac{t}{e^t} \ e^t \ dt$$ |
| | $$= 2 \int \frac{t-1}{t} \ dt$$ | $$= \int \frac{1}{1+t} \ dt$$ | $$= \int t \ dt$$ |
| 5. Evaluate the integral | $$2 \int \frac{t-1}{t} \ dt = 2 \int \left( 1-\frac{1}{t} \right) \ dt$$ | $$\int \frac{1}{1+t} \ dt = \ln(1+t)$$ | $$\int t \ dt = \frac{1}{2} t^2$$ |
| | $$= 2 \left( \int dt - \int \frac{dt}{t} \right) = 2(t-\ln(t))$$ | | |
| 6. Rewrite expressions in terms of $x$ | as $t = \sqrt{x}$: | as $t = e^x$: | as $t = \ln(x)$: |
| | $2(t-ln(t)) = 2(\sqrt{x}-\ln(\sqrt{x})$ | $\ln(1+t) = ln(1+e^x)$ | $\frac{1}{2} t^2 = \frac{1}{2} \ln^2(x)$ |
| | $\equiv 2\sqrt{x} - \ln(x)$ | | |
