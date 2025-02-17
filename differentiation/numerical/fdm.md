# Finite Difference Method

The **finite-difference method** (FDM) is a technique of numerical differentiation used to approximate derivative of a function.

Variants of the method:

- **central difference** (most accurate)

$$
f'(x) \approx \frac{f(x+h)-f(x-h)}{2h}
$$

- **forward difference**

$$
f'(x) \approx \frac{f(x+h)-f(x)}{h}
$$

- **backward difference**

$$
f'(x) \approx \frac{f(x)-f(x-h)}{h}
$$

> $h$ - a small numerical step
