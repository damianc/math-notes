# Hyperbolic Functions

## Definitions

| Function | Formula | Alt. Formula |
|--|--|--|
| $$\text{sinh}(x)$$ | $$\frac{1}{2}\left(e^x-e^{-x}\right)$$ | $$\frac{e^{2x}-1}{2e^x}$$ |
| $$\text{cosh}(x)$$ | $$\frac{1}{2}\left(e^x+e^{-x}\right)$$ | $$\frac{e^{2x}+1}{2e^x}$$ |
| $$\text{tanh}(x)$$ | $$\frac{e^x-e^{-x}}{e^x+e^{-x}}$$ | $$\frac{e^{2x}-1}{e^{2x}+1}$$ |
| $$\text{csch}(x)$$ | $$\frac{2}{e^x-e^{-x}}$$ | $$\frac{2e^x}{e^{2x}-1}$$ |
| $$\text{sech}(x)$$ | $$\frac{2}{e^x+e^{-x}}$$ | $$\frac{2e^x}{e^{2x}+1}$$ |
| $$\text{coth}(x)$$ | $$\frac{e^x+e^{-x}}{e^x-e^{-x}}$$ | $$\frac{e^{2x}+1}{e^{2x}-1}$$ |

## Domain and Range

| Function | Domain | Range |
|--|--|--|
| sinh | $\mathbb{R}$ | $\mathbb{R}$ |
| cosh | $\mathbb{R}$ | $\langle 1,\infty)$ |
| tanh | $\mathbb{R}$ | $(-1,1)$ |
| csch | $\mathbb{R} \setminus \\{0\\}$ | $\mathbb{R} \setminus \\{0\\}$ |
| sech | $\mathbb{R}$ | $(0,1 \rangle$ |
| coth | $\mathbb{R} \setminus \\{0\\}$ | $\mathbb{R} \setminus \langle -1,1 \rangle$ |
| | | $(-\infty,-1) \cup (1,\infty)$ |

## Reciprocal Identities

| | |
|--|--|
| $\text{sinh}(x) = \frac{1}{\text{csch} (x)}$ | $\text{csch}(x) = \frac{1}{\text{sinh} (x)}$ |
| $\text{cosh}(x) = \frac{1}{\text{sech} (x)}$ | $\text{sech}(x) = \frac{1}{\text{cosh} (x)}$ |
| $\text{tanh}(x) = \frac{1}{\text{coth} (x)}$ | $\text{coth}(x) = \frac{1}{\text{tanh} (x)}$ |

## Quotient Identities

| Function | Quotient | Alt. Quotient | Implied Product |
|--|--|--|--|
| **sinh(x)** | $$\frac{\text{tanh}\ x}{\text{sech}\ x}$$ | $$\frac{\text{cosh}\ x}{\text{coth}\ x}$$ | $$\text{cosh}(x)\ \text{tanh}(x)$$ |
| **cosh(x)** | $$\frac{\text{sinh}\ x}{\text{tanh}\ x}$$ | $$\frac{\text{coth}\ x}{\text{csch}\ x}$$ | $$\text{sinh}(x)\ \text{coth}(x)$$ |
| **tanh(x)** | $$\frac{\text{sinh}\ x}{\text{cosh}\ x}$$ | $$\frac{\text{sech}\ x}{\text{csch}\ x}$$ | $$\text{sinh}(x)\ \text{sech}(x)$$ |
| **csch(x)** | $$\frac{\text{sech}\ x}{\text{tanh}\ x}$$ | $$\frac{\text{coth}\ x}{\text{cosh}\ x}$$ | $$\text{sech}(x)\ \text{coth}(x)$$ |
| **sech(x)** | $$\frac{\text{tanh}\ x}{\text{sinh}\ x}$$ | $$\frac{\text{csch}\ x}{\text{coth}\ x}$$ | $$\text{tanh}(x)\ \text{csch}(x)$$ |
| **coth(x)** | $$\frac{\text{cosh}\ x}{\text{sinh}\ x}$$ | $$\frac{\text{csch}\ x}{\text{sech}\ x}$$ | $$\text{cosh}(x)\ \text{csch}(x)$$ |

## $\ln \varphi$ Identities

| | |
|--|--|
| $\sinh(\ln\varphi) = \frac{1}{2}$ | $\text{csch}(\ln\varphi) = 2$ |
| $\cosh(\ln\varphi) = \frac{\sqrt{5}}{2}$ | $\text{sech}(\ln\varphi) = \frac{2}{\sqrt{5}}$ |
| $\tanh(\ln\varphi) = \frac{1}{\sqrt{5}}$ | $\coth(\ln\varphi) = \sqrt{5}$ |

## Derivatives

| $\boldsymbol{f(x)}$ | $\boldsymbol {\frac{d}{dx} f(x)}$ |
|--|--|
| sinh | $\cosh(x)$ |
| cosh | $\sinh(x)$ |
| tanh | $\text{sech}^2(x)$ |
| csch | $-\coth(x) \text{csch}(x)$ |
| sech | $-\text{sech}(x) \tanh(x)$ |
| coth | $-\text{csch}^2(x)$ |

## Integrals

| $\boldsymbol{f(x)}$ | $\boldsymbol{\int f(x) \ dx}$ |
|--|--|
| sinh | $\cosh(x)+C$ |
| cosh | $\sinh(x)+C$ |
| tanh | $\ln(\cosh(x))+C$ |
| csch | $\ln\left(\tanh\left(\frac{x}{2}\right)\right)+C$ |
| sech | $2\arctan\left(\tanh\left(\frac{x}{2}\right)\right)+C$ |
| | $\cup \ \  \arctan(\sinh(x))+C$ |
| coth | $\ln(\sinh(x))+ C$ |


