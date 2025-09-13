# Trigonometric Functions

## Definitions

| Function | $f(x)$ | $f^{-1}(x)$ |
|--|--|--|
| sine | $\sin(x)$ | $\arcsin(x)$ |
| cosine | $\cos(x)$ | $\arccos(x)$ |
| tangent | $\tan(x)$ | $\arctan(x)$ |
| cosecant | $\csc(x) = \frac{1}{\sin(x)}$ | $\arcsin\left(\frac{1}{x}\right)$ |
| secant | $\sec(x) = \frac{1}{\cos(x)}$  | $\arccos\left(\frac{1}{x}\right)$ |
| cotangent | $\cot(x) = \frac{1}{\tan(x)}$ | $\arctan\left(\frac{1}{x}\right)$ |
| exsec[ant] (_external secant_) | $\text{exs}(x) = \frac{1}{\cos(x)}-1$ | $\text{arcsec}(x+1) = \arccos\left(\frac{1}{x+1}\right) = \arctan(\sqrt{x^2+2x})$ | 
| excosec[ant]/coexsec[ant] (_external cosecant_) | $\text{exc}(x) = \frac{1}{\sin(x)}-1$ | $\text{arccsc}(x+1) = \arcsin\left(\frac{1}{x+1}\right)$ |
| versin (_versed sine_) | $\text{ver}(x) = 2\sin^2\left(\frac{x}{2}\right) = 1-\cos(x)$ | $\arccos(1-x)$ |
| coversin (_coversed sine_) | $\text{cvs}(x) = 1-\sin(x)$ | $\arcsin(1-x)$ |
| vercos (_versed cosine_) | $\text{vcs}(x) = 2\cos^2\left(\frac{x}{2}\right) = 1+\cos(x)$ | $\arccos(x-1)$ |
| covercos (_coversed cosine_) | $\text{cvc}(x) = 1+\sin(x)$ | $\arcsin(x-1)$ |
| haversin (_half-versed sine_) | $\text{hav}(x) = \sin^2\left(\frac{x}{2}\right) = \frac{1-\cos(x)}{2}$ | $2\arcsin(\sqrt{x}) = \arccos(1-2x)$ |
| hacoversin (_half-coversed sine_) | $\text{hcv}(x) = \frac{1-\sin(x)}{2}$ | $\arcsin(1-2x)$ |
| havercos (_half-versed cosine_) | $\text{hvc}(x) = \cos^2\left(\frac{x}{2}\right) = \frac{1+\cos(x)}{2}$ | $2\arccos(\sqrt{x}) = \arccos(2x-1)$ |
| hacovercos (_half-coversed cosine_) | $\text{hcc}(x) = \frac{1+\sin(x)}{2}$ | $\arcsin(2x-1)$ |

> In terms of naming, _*sin_ = _*sine_, as well as _*cos_ = _*cosin(e)_.

## Domain and Range

### Primary Trigonometric Functions

| Function | Domain | Range | Inv. Function | Domain | Range |
|--|--|--|--|--|--|
| sine | ℝ | [-1,1] | arcus sine | [-1,1] | [-½π,½π] |
| cosine | ℝ | [-1,1] | arcus cosine | [-1,1] | [0,π] |
| tangent | {x ∈ ℝ: xπ⁻¹ + ½ ∉ ℤ} | ℝ | arcus tangent | ℝ | (-½π,½π) |

### Secondary Trigonometric Functions

| Function | Domain | Range | Inv. Function | Domain | Range |
|--|--|--|--|--|--|
| cosecant | {x ∈ ℝ: xπ⁻¹ ∉ ℤ} | ℝ\\(-1,1) | arcus cosecant | ℝ\\(-1,1) | [-½π,½π]\\{0} |
| secant | {x ∈ ℝ: xπ⁻¹ + ½ ∉ ℤ} | ℝ\\(-1,1) | arcus secant | ℝ\\(-1,1) | [0,π]\\{½π} |
| cotangent | {x ∈ ℝ: xπ⁻¹ ∉ ℤ} | ℝ | arcus cotangent | ℝ | (-½π,½π)\\{0} |

### Other Trigonometric Functions

| Function | Domain | Range | Inv. Function | Domain | Range |
|--|--|--|--|--|--|
| exsecant | {x ∈ ℝ: xπ⁻¹ + ½ ∉ ℤ} | ℝ\\(-2,0) | arcus exsecant | ℝ\\(-2,0) | [0,π]\\{½π} |
| excosecant | {x ∈ ℝ: xπ⁻¹ ∉ ℤ} | ℝ\\(-2,0) | arcus excosecant | ℝ\\(-2,0) | [-½π,½π]\\{0} |

#### [Co]Versed Functions


| Function | Domain | Range | Inv. Function | Domain | Range |
|--|--|--|--|--|--|
| versine | ℝ | [0,2] | arcus versine | [0,2] | [0,π] |
| coversine | ℝ | [0,2] | arcus coversine | [0,2] | [-½π,½π] |
| vercosine | ℝ | [0,2] | arcus vercosine | [0,2] | [0,π] |
| covercosine | ℝ | [0,2] | arcus covercosine | [0,2] | [-½π,½π] |

#### Half-[Co]Versed Functions


| Function | Domain | Range | Inv. Function | Domain | Range |
|--|--|--|--|--|--|
| haversine | ℝ | [0,1] | arcus haversine | [0,1] | [0,π] |
| hacoversine | ℝ | [0,1] | arcus hacoversine | [0,1] | [-½π,½π] |
| havercosine | ℝ | [0,1] | arcus havercosine | [0,1] | [0,π] |
| hacovercosine | ℝ | [0,1] | arcus hacovercosine | [0,1] | [-½π,½π] |
