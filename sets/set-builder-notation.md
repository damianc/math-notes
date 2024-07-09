# Set-Builder Notation

The following denotes the set formed by the values of $x$ for which $P(x)$ is _true_:

$$
\Large
\\{\ x\ |\ P(x)\ \\}
$$

- for example:

$$
\\{\ x\ |\ x \in [1,4]\ \\} =
\\{1,2,3,4\\}
$$

- `:` can be used instead of `|`:

$$
\\{\ x:\ x \in [1,4]\ \\} =
\\{1,2,3,4\\}
$$

## Examples

$$
\\{ x^2 \ |\ x \in [1,4] \\} =
\\{1,4,9,16\\}
$$

$$
\\{ x \in \mathbb{N} \ |\ x < 10 \\} =
\\{1,2,...,9\\}
$$

$$
\\{ x:\ x^2-4 = 0 \\} =
\\{ -2,2 \\}
$$

$$
\\{ x \in \mathbb{N}:\ x \propto k \\} =
\\{ 1k,2k,3k,4k,... \\}
$$

- the very first expression may be a polynomial:

$$
\\{ 2k+1 \ \|\ k \in \mathbb{N}_0 \\} =
\\{ 1,3,5,7,9,... \\}
$$

### Common and Useful Examples

| Example | Expression |
|--|--|
| even numbers | $\\{\ 2k \ \|\ k \in \mathbb{Z} \ \\}$ |
| | $\\{\ k \in \mathbb{Z} \ \|\ k \equiv 0 \pmod 2 \ \\}$ |
| odd numbers | $\\{\ 2k+1 \ \|\ k \in \mathbb{Z} \ \\}$ |
| | $\\{\ k \in \mathbb{Z} \ \|\ k \equiv 1 \pmod 2 \ \\}$ |
| prime numbers | $\\{\ p \in \mathbb{N} \ \|\ \forall(k \in \mathbb{N} \setminus \\{1,p\\})\left(\frac{p}{k} \notin \mathbb{Z}\right) \ \\}$ |
| roots of the function | $\\{\ x \ \|\ f(x) = 0 \ \\}$ |
| combinations | $\\{\ X \in {\cal P}(S): \|X\| = k \ \\}$ |
| | $\\{\ X \subseteq S: \|X\| = k \ \\}$ |
| points forming a circle | $\\{\ (x,y) \in \mathbb{R}^2 \ \|\ (x-a)^2+(y-b)^2=r^2 \land (a,b,r \in \mathbb{R}) \ \\}$ |
| | $\\{\ p \in \mathbb{R}^2 \ \|\ (p_1-a)^2+(p_2-b)^2=r^2 \land (a,b,r \in \mathbb{R}) \ \\}$ |

### Examples in Terms of Sequences

> $a_0$ - initial term in a sequence  
> $\Delta$ - common difference and ratio

| Sequence | Expression |
|--|--|
| arithmetic sequence with $n$ terms | $\\{\ a_0 + (k-1)\Delta \ \|\  k \in [1,n] \ \\}$ |
| artihmetic sequence going to $t$ | $\\{\ x_k \ \|\ x_k = a_0+(k-1)\Delta, k \in \mathbb{N}, x_k \leq t\ \\}$ |
| geometric sequence with $n$ terms | $\\{\ a_0\Delta^{k-1} \ \|\  k \in [1,n] \ \\}$ |
| geometric sequence going to $t$ | $\\{\ x_k \ \|\ x_k = a_0\Delta^{k-1}, k \in \mathbb{N}, x_k \leq t\ \\}$ |

### Examples in Terms of Set Operations

| Operation | Expression |
|--|--|
| $A \cup B$ | $\\{\ x: x \in A \lor x \in B \ \\}$ |
| $A \cap B$ | $\\{\ x: x \in A \land x \in B \ \\}$ |
| $A \setminus B$ | $\\{\ x \in A: x \notin B\ \\}$ |
| $A \mathop{\triangle} B$ | $\\{\ x: (x \in A \land x \notin B) \lor (x \in B \land x \notin A)\ \\}$ |
| $A \times B$ | $\\{\ (a,b): a \in A \land b \in B\ \\}$ |
| $A^{\complement}$ | $U \setminus A$ = $\\{\ x \in U: x \notin A\ \\}$ |
| ${\cal P}(A)$ | $\\{\ X: X \subseteq A\ \\}$ |

### Examples in Terms of Numbers Sets

| Set | Expression |
|--|--|
| $\mathbb{Z}$ | $\\{\ x \in \mathbb{R}: {\tt T}\left(\frac{x}{2}\right) \in \\{0,0.5\\}, {\tt T}(n) = n - \lfloor n \rfloor \ \\}$ |
| $\mathbb{Z}^{+}$ | $\\{\ x \in \mathbb{Z}: x \gt 0 \ \\}$ or $\\{\ x: x \in \mathbb{N} \ \\}$ |
| $\mathbb{N}$ | $\\{\ x \in \mathbb{Z}: x \gt 0 \ \\}$ |
| $\mathbb{N}_0$ | $\\{\ x \in \mathbb{N}: x \geq 0 \ \\}$ |
| $\mathbb{Q}$ | $\left\\{\ \frac{p}{q}: p,q \in \mathbb{Z}, q \neq 0 \ \right\\}$ |
| $\mathbb{I}$ | $\\{\ x \in \mathbb{R}: x \notin \mathbb{Q} \ \\}$ |
| $\mathbb{C}$ | $\\{\ a+bi: a,b \in \mathbb{R}, i^2 = -1 \ \\}$ |
| $\mathbb{R}$ | $\\{\ x: x \notin \mathbb{C} \ \\}$ |
| $\mathbb{R}^2$ | $\\{\ (x,y): x,y \in \mathbb{R} \ \\}$ |

## Predicate

### Predicate Location

- predicate in expression:

$$
\\{
x^2\ |\ x \in [1,4]
\\}
$$

- predicate out of expression:

$$
\\{
x^2\ |\ P(x)
\\}
$$

$$
P(x) = x \in [1,4]
$$

- predicate defined in expression:

$$
\\{
x^2 \ |\ P(x), P(x) = x \in [1,4]
\\}
$$

> every of the above yields $\\{ 1,4,9,16 \\}$

### Multiple Predicates

$$
\\{\ x_i \ \|\  {\tt P}_1(x_i)
\land {\tt P}_2(i)
\ \\}
$$

- example that yields $\\{2,6,10,14\\}$:

$$
\\{ x_i \in \mathbb{N} \ \|\ {\tt C_t}(x_i) \land
{\tt C_i}(i) \ \\}
$$

$$
{\tt C_t}(x_i) = (x_i = 2+4(i-1))
$$

$$
{\tt C_i}(i) = i \in [1,4]
$$

### Predicate Components

| Component | Example |
|--|--|
| equality | $x=1$ |
| inequality | $x \neq 0$ |
| | $x \gt 1$ |
| | $1 \leq x \leq 9$ |
| membership | $x \in [1,9]$ |
| | $P \in \mathbb{R}^2$ |
| | $x \notin S$ |
| divisibility | $2 \| x$ |
| | $x \equiv 0 \pmod 2$ |
| proportionality | $x \propto 4$ |
| logic _or_ | $x < 1 \lor x > 1$ |
| logic _and_ | $x \geq 10 \land x \propto 5$ |
| logic _not_ | $\lnot(x \propto k)$ |
| perpendicularity | $k_i \perp l_i$ |
| parallelity | $k_i \parallel \ell_i$ |
| cardinality of set | $\|S\| = 2$ |
| | $\\#S = 2$ |
| set relation | $A \subset B$ |
| | $S \subseteq \Omega$ |
| function | $f(x) = 0$ |
| | $\|\sin(x)\| \neq 1$ |
| set | $n \in \mathbb{N}^{+}$ |
| | $p_n \in {\cal P}(\omega_n)$ |

## Quantifiers

- $\forall n \in S$ - the universal quantifier that reads _"for all"_
- $\exists n \in S$ - the existential quantifier that reads _"exists such"_

### Examples Using Quantifiers

- every term $x$ from $S_1$ for which there is term $k$ from $S_2$ such that $T(x,k)$ returns _true_

$$
\\{\ x \in S_1: (\exists k \in S_2)(T(x,k)) \ \\}
$$

- every term $x$ from $S_1$ for which all terms $k$'s of $S_2$ satisfy $T(x,k)$

$$
\\{\ x \in S_1: (\forall k \in S_2)(T(x,k)) \ \\}
$$

> membership must be specified for a term bound to a quantifier: e.g., $\exists n \in \mathbb{N}$ is proper, while $\exists n$ not

