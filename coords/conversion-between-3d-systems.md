# Conversion between 3D Coordinates Systems

## Cartesian and Cylindrical

### Cartesian to Cylindrical

$$
\begin{array}{l}
(x,y,z) \mapsto (r,\theta,z)
\\
\ 
\\
r = \sqrt{x^2+y^2}
\\
\theta = \text{atan2}(y,x)
\\
z = z
\end{array}
$$

### Cylindrical to Cartesian

$$
\begin{array}{l}
(r,\theta,z) \mapsto (x,y,z)
\\
\ 
\\
x = r \cos(\theta)
\\
y = r \sin(\theta)
\\
z = z
\end{array}
$$

## Cartesian and Spherical

### Cartesian to Spherical

$$
\begin{array}{l}
(x,y,z) \mapsto (\rho,\theta,\phi)
\\
\ 
\\
\rho = \sqrt{x^2+y^2+z^2}
\\
\theta = \text{atan2}(y,x)
\\
\phi = \arccos\left(\frac{z}{\rho}\right)
\end{array}
$$

### Spherical to Cartesian

$$
\begin{array}{l}
(\rho,\theta,\phi) \mapsto (x,y,z)
\\
\ 
\\
x = \rho \sin(\phi) \cos(\theta)
\\
y = \rho \sin(\phi) \sin(\theta)
\\
z = \rho \cos(\phi)
\end{array}
$$

## Cylindrical and Spherical

### Cylindrical to Spherical
$$
\begin{array}{l}
(r,\theta,z) \mapsto (\rho,\theta,\phi)
\\
\ 
\\
\rho = \sqrt{r^2+z^2}
\\
\theta = \theta
\\
\phi = \arctan\left(\frac{r}{z}\right)
\end{array}
$$

### Spherical to Cylindrical

$$
\begin{array}{l}
(\rho,\theta,\phi) \mapsto (r,\theta,z)
\\
\ 
\\
r = \rho \sin(\phi)
\\
\theta = \theta
\\
z = \rho \cos(\phi)
\end{array}
$$

