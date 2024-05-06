# Box Construction

Construct a box with maximum possible volume.

![Assembled box](https://github.com/damianc/math-notes/blob/master/_images/pract/box/box-done.png) 

| | |
|--|--|
| | ![Square plane](https://github.com/damianc/math-notes/blob/master/_images/pract/box/box-plane-sq.png) |
| square plane | $$x = \frac{1}{6}a$$ |
| | ![Rectangular plane](https://github.com/damianc/math-notes/blob/master/_images/pract/box/box-plane-rect.png) |
| rectangular plane | $$x = \frac{1}{6}\left[a+b+\sqrt{\Delta}\right]$$ |
| | $$\cup^{\ *}$$ |
| | $$x = \frac{1}{6}\left[a+b-\sqrt{\Delta}\right]$$ |
| | $$\iff$$ |
| | $$\Delta = (a+b)^2 - 3ab$$ |
| | * - depending on which belongs to $\left( 0; \frac{\min(a,b)}{2}\right)$ |

## Proof

Getting proper values comes down to three steps:

- convert _volume formula_ to a _cubic function_
- get its _derivative_ (being a _quadratic function_)
- get _roots_ and pick a reasonable one
