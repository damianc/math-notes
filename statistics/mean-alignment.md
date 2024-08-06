# Mean Alignment

$$
\begin{array}{|c|c|ccc|c|c|}
x_1 & x_2 && \cdots && x_n & \nabla
\\
\hline
w_1 & w_2 && \cdots && w_n & \lambda
\end{array}
$$

## New value $\nabla$ (with optional weight $\lambda$) to set mean $\hat{x}$

| Type | $\nabla$ | $\nabla_W$ |
|--|--|--|
| arithmetic | $$\hat{x}(n+1)-\Sigma x$$ | $${\large \lambda}^{-1} \cdot \left[ \hat{x}\left(\lambda + \Sigma w\right) - \Sigma xw \right]$$ |
| geometric | $$\cfrac{\hat{x}^{n+1}}{\Pi x}$$ | $$\sqrt[\lambda]{\cfrac{\hat{x}^{\lambda+\Sigma w}}{\Pi x^w}}$$ |
| harmonic | $$\left( \frac{n+1}{\hat{x}} - \sum \frac{1}{x} \right)^{-1}$$ | $${\large\lambda} \cdot \left( \frac{\lambda+\Sigma w}{\hat{x}} - \sum \frac{w}{x} \right)^{-1}$$ |
| power | $$\sqrt[p]{\hat{x}^p(n+1)-\Sigma x^p}$$ | $$\sqrt[p]{{\large\lambda}^{-1} \cdot \left[ \hat{x}^p(\lambda+\Sigma w) - \Sigma wx^p \right]}$$ |
| root | $$\left( \sqrt[d]{\hat{x}}(n+1)-\Sigma \sqrt[d]{x} \right)^d$$ | $$\left( {\large\lambda}^{-1} \cdot \left[ \sqrt[d]{\hat{x}} \left( {\large\lambda}+\sum w \right) - \sum w \sqrt[d]{x} \right] \right)^d$$ |
| logarithmic | $${\large b}^{(n+1)\ln(\hat{x})-\Sigma \log_b(x)}$$ | $$\sqrt[\lambda]{{\large b}^{(\lambda+\Sigma w)\ln(\hat{x})-\Sigma w \log_b(x)}}$$ |

## Weight $\lambda$ of new value $\nabla_W$ to set mean $\hat{x}$

| Type | $\lambda$ |
|--|--|
| arithmetic | $$\frac{\hat{x}[\Sigma w] - \Sigma xw}{\nabla-\hat{x}} = \frac{\Sigma w(\hat{x}-x)}{\nabla-\hat{x}}$$ |
| geometric | $$\frac{\ln(\Pi x^w)-[\Sigma w]\ln(\hat{x})}{\ln(\hat{x})-\ln(\nabla)}$$ |
| harmonic | $$\frac{\nabla\left(\left[\sum w\right]-\hat{x}\sum\frac{w}{x}\right)}{\hat{x}-\nabla}$$ |
| power | $$\frac{\hat{x}^p[\Sigma w]-\Sigma wx^p}{\nabla^p-\hat{x}^p}$$ |
| root | $$\frac{\sqrt[d]{\hat{x}}[\Sigma w]-\Sigma w \sqrt[d]{x}}{\sqrt[d]{\nabla}-\sqrt[d]{\hat{x}}}$$ |
| logarithmic | $$\frac{[\Sigma w]\ln(\hat{x})-\log_b(\Pi x^w)}{\log_b(\nabla)-\ln(\hat{x})}$$ |


