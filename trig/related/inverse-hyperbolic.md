# Inverse Hyperbolic Functions

## Definitions

| Function | Formula |
|--|--|
| $$\text{asinh}(x)$$ | $$\ln(x+\sqrt{x^2+1})$$ |
| $$\text{acosh}(x)$$ | $$\ln(x+\sqrt{x-1}\sqrt{x+1})$$ |
| $$\text{atanh}(x)$$ | $$\frac{1}{2}\left[\ln(1+x)-\ln(1-x)\right]$$ |
| $$\text{acsch}(x)$$ | $$\ln\left(\sqrt{\frac{1}{x^2}+1}+\frac{1}{x}\right)$$ |
| $$\text{asech}(x)$$ | $$\ln\left(\sqrt{\frac{1}{x}-1}\sqrt{\frac{1}{x}+1}+\frac{1}{x}\right)$$ |
| $$\text{acoth}(x)$$ | $$\frac{1}{2}\left[\ln\left(1+\frac{1}{x}\right)-\ln\left(1-\frac{1}{x}\right)\right]$$ |

## Domain and Range

| Function | Domain | Range |
|--|--|--|
| asinh | $\mathbb{R}$ | $\mathbb{R}$ |
| acosh | $\langle 1,\infty )$ | $\langle 0,\infty )$ |
| atanh | $(-1,1)$ | $\mathbb{R}$ |
| acsch | $\mathbb{R} \setminus \\{0\\}$ | $\mathbb{R} \setminus \\{0\\}$ |
| asech | $(0,1\rangle$ | $\langle 0,\infty )$ |
| acoth | $\mathbb{R} \setminus \langle -1,1 \rangle$ | $\mathbb{R} \setminus \\{0\\}$ |

## Derivatives

| $\boldsymbol{f(x)}$ | $\boldsymbol{\frac{d}{dx} f(x)}$ |
|--|--|
| asinh | $$\frac{1}{\sqrt{x^2+1}}$$ |
| acosh | $$\frac{1}{\sqrt{x-1}\sqrt{x+1}}$$ |
| atanh | $$\frac{1}{1-x^2}$$ |
| acsch | $$-\frac{1}{\sqrt{\frac{1}{x^2}+1} \ \ x^2}$$ |
| asech | $$-\frac{1}{\sqrt{\frac{1}{x}-1}\sqrt{\frac{1}{x}+1}\ \  x^2}$$ |
| acoth | $$\frac{1}{1-x^2}$$ |

## Integrals

| $\boldsymbol{f(x)}$ | $\boldsymbol{\int f(x) dx}$ |
|--|--|
| asinh | $$x\ \text{asinh}(x)-\sqrt{x^2+1} + C$$ |
| acosh | $$x\ \text{acosh}(x)-\sqrt{x-1}\sqrt{x+1} + C$$ |
| atanh | $$\frac{1}{2} \ln(1-x^2)+x\ \text{atanh}(x) + C$$ |


