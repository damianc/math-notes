# Multiple Integrals Rules

## Sum/Difference Rule

Integral of a sum/difference is a sum/difference of integrals:

$$
\int \int_D f(x,y) \pm g(x,y) \ dA = \int \int_D f(x,y) \ dA \pm \int \int_D g(x,y) \ dA
$$

for example:

$$
\int_0^1 \int_2^3
x^2+y^2 \ dx \ dy =
\int_0^1 \int_2^3
x^2 \ dx \ dy +
\int_0^1 \int_2^3
y^2 \ dx \ dy
$$

## Constant Multiple Rule

A constant factor goes before integral:

$$
\int \int_D k f(x,y) \ dA = k \int \int_D f(x,y) \ dA
$$

for example:

$$
\int_0^1 \int_2^3 2xy \ dx \ dy =
2 \int_0^1 \int_2^3 xy \ dx \ dy
$$

## Additivity Rule

An integral over an area can be split up into sum of integrals over its sub-regions:

$$
\int \int_D f(x,y) \ dA = \int \int_{D_1} f(x,y) \ dA + \int \int_{D_2} f(x,y) \ dA
$$

$$
\iff
$$

$$
D_1 \cup D_2 = D
\ \bigwedge \ 
D_1 \cap D_2 = \varnothing
$$

### Generalization

For $I = \\{ 1,2,\dots,n \\}$:

$$
\begin{array}{rl}
{\displaystyle \int \int_D} f(x,y) \ dA = &
\displaystyle\sum_{i \in I} {\displaystyle \int \int_{D_i}} f(x,y) \ dA =
\\
\ 
\\
& {\displaystyle \int \int_{D_1}} f(x,y) \ dA \ +
\\
& {\displaystyle \int \int_{D_2}} f(x,y) \ dA \ +
\\
& \cdots \ +
\\
& {\displaystyle \int \int_{D_n}} f(x,y) \ dA
\end{array}
$$

$$
\iff
$$

$$
\left[
\ \underset{i \in I}{\bigcup} \ D_i\ 
\right] = D
\ \bigwedge \ 
\underset{
 \substack{
  i \in I
  \\
  j \in I \setminus \\{i\\}
 }
}{\Large\forall}
D_i \cap D_j = \varnothing
$$

### Example

The following area:

$$
\int_0^2 \int_0^2
$$

Can be split up in various ways, three examples are:

- two vertical parts

$$
\int_0^2 \int_0^1 + \int_0^2 \int_1^2
$$

- two horizontal parts

$$
\int_0^1 \int_0^2 + \int_1^2 \int_0^2
$$

- four quarters

$$
\int_0^1 \int_0^1 + \int_0^1 \int_1^2 +
\int_1^2 \int_0^1 + \int_1^2 \int_1^2
$$
