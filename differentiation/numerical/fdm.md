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

## Partial Derivatives

When handling partial derivatives, we only shift a variable the differentation is performed with respect to. For _central difference_ it goes as follows:

$$
\frac{\partial}{\partial x} f(x,y,z) \approx \frac{f(x+h,y,z)-f(x-h,y,z)}{2h}
$$

$$
\frac{\partial}{\partial y} f(x,y,z) \approx \frac{f(x,y+h,z)-f(x,y-h,z)}{2h}
$$

$$
\frac{\partial}{\partial z} f(x,y,z) \approx \frac{f(x,y,z+h)-f(x,y,z-h)}{2h}
$$

### Implementation

In the implementaion below, the `varIndex` is assigned value $0$ if we perform differentation with respect to variable $x$; $1$ is for variable $y$, and $2$ is for variable $z$.

```
function fdm(f,varIndex) {
  return (x,y,z) => {
    const h = 0.001;
    const arg = [0,0,0];
    arg[varIndex] = h;
  
    const [dx,dy,dz] = arg;
    const R = f(x+dx,y+dy,z+dz);
    const L = f(x-dx,y-dy,z-dz);
    
    return (R-L)/(2*h);
  };
}
```

## Higher-Order Derivatives

### Second-Order Derivatives

- **central difference**

$$
f''(x) \approx \frac{
f(x+h)-2f(x)+f(x-h)
}{h^2}
$$

- **forward difference**

$$
f''(x) \approx \frac{
f(x+2h)-2f(x+h)+f(x)
}{h^2}
$$

- **backward difference**

$$
f''(x) \approx \frac{
f(x)-2f(x-h)+f(x-2h)
}{h^2}
$$

### Third-Order Derivatives

- **central difference**

$$
f'''(x) \approx \frac{
f(x+2h)-2f(x+h)+2f(x-h)-f(x-2h)
}{2h^3}
$$

- **forward difference**

$$
f'''(x) \approx \frac{
f(x+3h)-3f(x+2h)+3f(x+h)-f(x)
}{h^3}
$$

- **backward difference**

$$
f'''(x) \approx \frac{
f(x)-3f(x-h)+3f(x-2h)-f(x-3h)
}{h^3}
$$
