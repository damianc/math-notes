# Circle Parameters

| Parameter | Formula | Getting r from Parameter | Getting $\alpha$ from Parameter |
|--|:--:|:--:|:--:|
| circumference | $2{\pi}r$ | $\frac{x}{2\pi}$ | - |
| area | ${\pi}r^2$ | $\sqrt{\frac{x}{\pi}}$ | - |
| arc length | ${\alpha}r$ | $\frac{x}{\alpha}$ | $\frac{x}{r}$ |
| chord length | $2r \sin(\frac{\alpha}{2})$ | $\frac{x}{2 \sin(\frac{\alpha}{2})}$ | $2 \arcsin(\frac{x}{2r})$ |
| sector area | $\frac{\alpha}{2} r^2$ | $\sqrt{\frac{2x}{\alpha}}$ | $2 \frac{x}{r^2}$ |
| segment area | $\frac{r^2}{2}(\alpha - \sin(\alpha))$ | $\sqrt{2\frac{x}{\alpha - \sin(\alpha)}}$ | by *numeral methods* |
| perpendicular distance from circle center to chord | $r \cos(\frac{\alpha}{2})$ | $\frac{x}{\cos(\frac{\alpha}{2})}$ | $2 \arccos(\frac{x}{r})$ |
| perpendicular distance from circle edge to chord | $r - r \cdot \cos\left(\frac{\alpha}{2}\right)$ | $-x \cdot \frac{1}{\cos\left(\frac{\alpha}{2}\right)-1}$ | $2 \arccos\left(\frac{-x+r}{r}\right)$ |
