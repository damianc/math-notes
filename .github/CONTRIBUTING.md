# Contributing Rules

Be explicit:

| NOT OK | OK |
|--|--|
| $a\frac{b}{c}$ | $a \cdot \frac{b}{c}$, $a + \frac{b}{c}$ |
| $\sin^{-1}(x)$ | $\text{asin}(x)$ or $\arcsin(x)$, $\csc(x)$ |
| $\log(x)$ | $\ln(x)$, $\log_{10}(x)$ |
| $\sin \ x+k$ | $\sin(x+k)$, $\sin(x)+k$ |

- for natural numbers including 0:

$$
\Bbb{N}_0
$$



## Allowed Descriptors

### Functions

Stick to the list below. Strange stuff like _tg_, _ctg_ or _lb_ is not allowed.

| Function | Allowed descriptor(s) |
|--|--|
| sine | $\sin$ |
| cosine | $\cos$ |
| tangent | $\tan$ |
| cosecant | $\csc$ |
| secant | $\sec$ |
| cotangent | $\cot$ |
| arcus sine (etc.) | $\text{asin}$ or $\arcsin$ (etc.) |
| hyperbolic sine (etc.) | $\sinh$ (etc.) |
| inverse hyperbolic sine (etc.) | $\text{asinh}$ or $\text{arcsinh}$ (etc.) |
| natural logarithm | $\ln$ |
| n-base logarithm | $\log_n$ (e.g., $\log_2$, $\log_{10}$ etc.) |
| least/lowest common multiple | $\text{lcm}$ or $\text{LCM}$ |
| lowest/least common denominator | $\text{lcd}$ or $\text{LCD}$ |
| greatest common divisor/factor | $\gcd$ or $\text{GCD}$ |
| determinant | $\det$ |
| degree | $\deg$ |
| gradient | $\text{grad}(f)$ or $\nabla f$ |
| divergence | $\text{div}(F)$ or $\nabla \cdot F$ |
| curl/rotation | $\text{curl}(F)$ or $\nabla \times F$ |

Rarely used trigonometric functions:

| Function | Allowed descriptor | Definition |
|--|--|--|
| excosecant/coexsecant (_external cosecant_) | exc | exc(x) = csc(x)-1 |
| exsecant (_external secant_) | exs | exs(x) = sec(x)-1 |
| versin (_versed sine_) | ver | ver(x) = 1-cos(x) |
| coversin (_coversed sine_) | cvs | cvs(x) = 1-sin(x) |
| vercos (_versed cosine_) | vcs | vcs(x) = 1+cos(x) |
| covercos (_coversed cosine_) | cvc | cvc(x) = 1+sin(x) |
| haversin (_half-versed sine_) | hav | hav(x) = ½ver(x) |
| hacoversin (_half-coversed sine_) | hcv | hcv(x) = ½cvs(x) |
| havercos (_half-versed cosine_) | hvc | hvc(x) = ½vcs(x) |
| hacovercos (_half-coversed cosine_) | hcc | hcc(x) = ½cvc(x) |

### Sets

| Numbers | Descriptor | Info to add |
|--|--|--|
| real | $\Bbb{R}$ | |
| complex | $\Bbb{C}$ | |
| integer | $\Bbb{Z}$ | |
| rational | $\Bbb{Q}$ | |
| natural | $\Bbb{N}$ | |
| natural with 0 | $\Bbb{N}_0$ | |
| positive real (etc.) | $\Bbb{R}^{+}$ (etc.) |  whether or not with 0 |
| negative real (etc.) | $\Bbb{R}^{-}$ (etc.) | whether or not with 0 |
| non-negative real (etc.) | $\Bbb{R}_0^{+}$ (etc.) | |
| non-positive real (etc.) | $\Bbb{R}_0^{-}$ (etc.) | |

Sets should be defined with the **set-builder notation**, for example:

$$
E^{+} = \\{ 2n \in \Bbb{N} \ | \ n \geq 0 \\}
$$

As simple set as an arithmeric sequence can be defined in a convenient manner like below:

- $\\{ 1,2, \ \dots \ n \\}$ or $\\{ 1,2, \ \dots \\}$
- $\\{ 1,1.5,2, \ \dots \ n \\}$ or $\\{ 1,1.5,2, \ \dots \\}$

Following descriptors can be used as long as there is explanation accompanying:

- $\Bbb{P}$ for prime numbers
- $\Bbb{E}$ for even numbers
- $\Bbb{O}$ for odd numbers
- $\Bbb{I}$ for imaginary numbers ($0+bi$)

