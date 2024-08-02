# Means

| Type | Formula | Weighted variant |
|--|--|--|
| arithmetic | $$\frac{\sum x}{n}$$ | $$\frac{\sum xw}{\sum w}$$ |
| geometric | $$\sqrt[n]{\prod x}$$ | $$\sqrt[\sum w]{\prod x^w}$$ |
| harmonic | $$n \cdot \left[ \sum \frac{1}{x} \right]^{-1}$$ | $$\left[ \sum w \right] \cdot \left[ \sum \frac{w}{x} \right]^{-1}$$ |
| power $$\ $$ (of $p$) | $$\sqrt[p]{\frac{\sum x^p}{n}}$$ | $$\sqrt[p]{\frac{\sum x^p \cdot w}{\sum w}}$$ |
| root (with degree $d$) | $$\left(\frac{\sum \sqrt[d]{x}}{n}\right)^d$$ | $$\left(\frac{\sum \sqrt[d]{x} \cdot w}{\sum w}\right)^d$$ |
| logarithmic (with base $b$) | $$e^{\square}, \square = \frac{\sum \log_b(x)}{n}$$ | $$e^{\square}, \square = \frac{\sum \log_b(x) \cdot w}{\sum w}$$ |

> $\sum \log_b(x) {\color{#aaa} \cdot w}$ can be replaced with $\log_b\left( \prod x^{\color{#aaa} w} \right)$
