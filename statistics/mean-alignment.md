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
| arithmetic | $$\hat{x}(n+1)-\Sigma x$$ | $$\frac{1}{\lambda}\left[ \hat{x}\left(\lambda + \Sigma w\right) - \Sigma xw \right]$$ |
| geometric | $$\cfrac{\hat{x}^{n+1}}{\Pi x}$$ | $$\sqrt[\lambda]{\cfrac{\hat{x}^{\lambda+\Sigma w}}{\Pi x^w}}$$ |
| harmonic | $$\left( \frac{n+1}{\hat{x}} - \sum \frac{1}{x} \right)^{-1}$$ | $${\large\lambda}\left( \frac{\lambda+\Sigma w}{\hat{x}} - \sum \frac{w}{x} \right)^{-1}$$ |
| power | $$\sqrt[p]{\hat{x}^p(n+1)-\Sigma x^p}$$ | $$\sqrt[p]{\frac{1}{\lambda}\left[ \hat{x}^p(\lambda+\Sigma w) - \Sigma wx^p \right]}$$ |
