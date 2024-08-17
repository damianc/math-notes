# Means

| Type | Formula | Weighted variant |
|--|--|--|
| arithmetic | $$\overline{x}_{\tiny A} = \frac{\sum x}{n}$$ | $$\overline{x}_{\tiny WA} = \frac{\sum xw}{\sum w}$$ |
| geometric | $$\overline{x}_{\tiny G} = \sqrt[n]{\prod x}$$ | $$\overline{x}_{\tiny WG} = \sqrt[\sum w]{\prod x^w}$$ |
| harmonic | $$\overline{x}_{\tiny H} = n \cdot \left[ \sum \frac{1}{x} \right]^{-1}$$ | $$\overline{x}_{\tiny WH} = \left[ \sum w \right] \cdot \left[ \sum \frac{w}{x} \right]^{-1}$$ |
| power (of $p$) | $$\overline{x}_{\tiny P(p)} = \sqrt[p]{\frac{\sum x^p}{n}}$$ | $$\overline{x}_{\tiny WP(p)} = \sqrt[p]{\frac{\sum x^p \cdot w}{\sum w}}$$ |
| root (with degree $d$) | $$\overline{x}_{\tiny R(d)} = \left(\frac{\sum \sqrt[d]{x}}{n}\right)^d$$ | $$\overline{x}_{\tiny WR(d)} = \left(\frac{\sum \sqrt[d]{x} \cdot w}{\sum w}\right)^d$$ |
| logarithmic (with base $b$) | $$\overline{x}_{\tiny L(b)} = e^{\square}, \square = \frac{\sum \log_b(x)}{n}$$ | $$\overline{x}_{\tiny WL(b)} = e^{\square}, \square = \frac{\sum \log_b(x) \cdot w}{\sum w}$$ |
| contraharmonic (Lehmer mean with $p=2$) | $$\overline{x}_{\tiny C} = \frac{\Sigma x^2}{\Sigma x}$$ | $$\overline{x}_{\tiny WC} = \frac{\Sigma wx^2}{\Sigma wx}$$ |
| Lehmer | $$\overline{x}_{\tiny Lh(p)} = \frac{\Sigma x^p}{\Sigma x^{p-1}}$$ | $$\overline{x}_{\tiny WLh(p)} = \frac{\Sigma wx^p}{\Sigma wx^{p-1}}$$ |
| generalized _f_-mean (with function $f(x)$ ) | $$\overline{x}_{\tiny F(f)} = f^{-1}\left( \frac{\Sigma f(x)}{n} \right)$$ | $$\overline{x}_{\tiny WF(f)} = f^{-1}\left( \frac{\Sigma w \cdot f(x)}{\Sigma w} \right)$$ |

> $\sum \log_b(x) {\color{#aaa} \cdot w}$ can be replaced with $\log_b\left( \prod x^{\color{#aaa} w} \right)$ (it also applies to $\ln$)
