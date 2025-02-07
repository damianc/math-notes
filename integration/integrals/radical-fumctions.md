# Integrals of Radical Functions

| $\boldsymbol{f(x)}$ | $\boldsymbol{\int f(x) \ dx}$ |
|--|--|
| $\sqrt{x}$ | $$\frac{2x^{3/2}}{3}$$ |
| $\sqrt{k+nx}$ | $$\frac{2(k+nx)^{3/2}}{3n}$$ |
| $\sqrt{k+nx^2}$ | $$\frac{1}{2}\left( x\sqrt{k+nx^2} - \frac{k\ln(\sqrt{k+nx^2}-\sqrt{n}x)}{\sqrt{n}} \right)$$ |
| $$\frac{1}{\sqrt{x}}$$ | $$2\sqrt{x}$$ |
| $$\frac{1}{\sqrt{k+nx}}$$ | $$\frac{2\sqrt{k+nx}}{n}$$ |
| $$\frac{1}{\sqrt{k+nx^2}}$$ | $$\frac{\text{atanh}\left(\frac{\sqrt{n}x}{\sqrt{k+nx^2}}\right)}{\sqrt{n}}$$ |

## Radical in Nominator

| $\boldsymbol{f(x)}$ | $\boldsymbol{\int f(x) \ dx}$ |
|--|--|
| $$\frac{\sqrt{nx+k}}{x}$$ | $$2\sqrt{k+nx}-2\sqrt{k} \text{atanh}\left( \frac{\sqrt{k+nx}}{\sqrt{k}} \right)$$ |
| $$\frac{nx^2+k}{x}$$ | $$\sqrt{k+nx^2}-\sqrt{k} \text{atanh}\left( \frac{\sqrt{k+nx^2}}{\sqrt{k}} \right)$$ |
| $$\frac{\sqrt{nx+k}}{x^2}$$ | $$-\frac{nx\nabla \text{atanh}(\nabla)+k+nx}{x\sqrt{k+nx}}, \nabla=\sqrt{\frac{nx}{k}+1}$$ |
| $$\frac{\sqrt{nx^2+k}}{x^2}$$ | $$-\frac{\sqrt{k+nx^2}+\sqrt{n}x \ln(\sqrt{k+nx^2}-\sqrt{n}x)}{x}$$ |

## Radical in Denominator

| $\boldsymbol{f(x)}$ | $\boldsymbol{\int f(x) \ dx}$ |
|--|--|
| $$\frac{x}{\sqrt{nx+k}}$$ | $$\frac{2(nx-2k)\sqrt{k+nx}}{3n^2}$$ |
| $$\frac{x}{\sqrt{nx^2+k}}$$ | $$\frac{\sqrt{k+nx^2}}{n}$$ |
| $$\frac{x^2}{\sqrt{nx+k}}$$ | $$\frac{2\sqrt{k+nx}(8k^2-4knx+3n^2x^2)}{15n^3}$$ |
| $$\frac{x^2}{\sqrt{nx^2+k}}$$ | $$\frac{\sqrt{n}x \sqrt{k+nx^2}+k \ln(\sqrt{k+nx^2}-\sqrt{n}x)}{2n^{3/2}}$$ |
