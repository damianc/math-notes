# Set-Builder Notation

The following denotes the set formed by the values of $x$ for which $P(x)$ is _true_:

$$
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

> both of the above yields $\\{ 1,4,9,16 \\}$

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
| | $p_n \in {\cal P}(\omega_n) \setminus \varnothing$ |

