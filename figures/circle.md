# Circle Parameters

| Parameter | Formula | Getting r from Parameter | Getting $\alpha$ from Parameter |
|--|:--:|:--:|:--:|
| circumference | $2{\pi}r$ | $\frac{x}{2\pi}$ | - |
| area | ${\pi}r^2$ | $\sqrt{\frac{x}{\pi}}$ | - |
| arc length | ${\alpha}r$ | $\frac{x}{\alpha}$ | $\frac{x}{r}$ |
| chord length | $2r \cdot \sin(\frac{\alpha}{2})$ | $\frac{x}{2 \sin(\frac{\alpha}{2})}$ | $2 \cdot \arcsin(\frac{x}{2r})$ |
| sector area | $\frac{1}{2} \alpha r^2$ | $\sqrt{\frac{2x}{\alpha}}$ | $\frac{2x}{r^2}$ |
| segment area | $\frac{1}{2}r^2(\alpha - \sin(\alpha))$ | $\sqrt{\frac{2x}{\alpha - \sin(\alpha)}}$ | by *numeral methods* |
| perpendicular distance from circle center to chord | $r \cdot \cos(\frac{\alpha}{2})$ | $\frac{x}{\cos(\frac{\alpha}{2})}$ | $2 \cdot \arccos(\frac{x}{r})$ |
| perpendicular distance from circle edge to chord | $\left(1-\cos\left(\frac{\alpha}{2}\right)\right)r$ | $\frac{x}{1-\cos\left(\frac{\alpha}{2}\right)}$ | $2 \cdot \arccos\left(1-\frac{x}{r}\right)$ |