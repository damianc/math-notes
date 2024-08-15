# Generalized Union and Intersection of Sets

- generalized union:

$$
\bigcup_{n=1}^k A_n = A_1 \cup A_2 \cup \cdots \cup A_k
$$

- generalized intersection:

$$
\bigcap_{n=1}^k A_n = A_1 \cap A_2 \cap \cdots \cap A_k
$$

## Other Forms

| Union | Intersection |
|--|--|
| $$\bigcup_{n \in \Bbb N} A_n = \bigcup_{n=1}^{\infty} A_n$$ | $$\bigcap_{n \in \Bbb N} A_n = \bigcap_{n=1}^{\infty} A_n$$ |
| $$\bigcup_{n \in T} A_n = \bigcup_{n=1}^{\vert T \vert} A_n$$ | $$\bigcap_{n \in T} A_n = \bigcap_{n=1}^{\vert T \vert} A_n$$ |
| $$\bigcup_{1 \le n \le k} A_n = \bigcup_{n=1}^k A_n$$ | $$\bigcap_{1 \le n \le k} A_n = \bigcap_{n=1}^k A_n$$ |

## Membership Properties

- generalized union:

$$
\left( x \in \bigcup_{t \in T} A_t \right)
\iff
\underset{t \in T}{\large\exists}
\left( x \in A_t \right)
$$

$$
\left( x \notin \bigcup_{t \in T} A_t \right)\iff\underset{t \in T}{\large\forall}\left( x \notin A_t \right)
$$

- generalized intersection:

$$
\left( x \in \bigcap_{t \in T} A_t \right)
\iff
\underset{t \in T}{\large\forall}
\left( x \in A_t \right)
$$

$$
\left( x \notin \bigcap_{t \in T} A_t \right)
\iff
\underset{t \in T}{\large\exists}
\left( x \notin A_t \right)
$$

> **simply put:**
> - $x$ belongs to a union if it is present in _at least one subset_ of a family
> - $x$ belongs to an intersection if it is present in _every subset_ of the family

## Examples

### Example 1

indexing set:  
$I = \\{ 1,2 \\}$

indexed family:  
${\cal F} = \\{ A_i \\}_{i \in I} = \\{ A_1,A_2 \\}$

_i-th_ term of ${\cal F}$:  
$A_i = \\{ i,2i \\}$

terms of ${\cal F}$:

$$
\begin{array}{rcl}
A_1 & = & \\{ 1,2 \\}
\\
A_2 & = & \\{ 2,4 \\}
\end{array}
$$

generalized union and intersection:

$$
\begin{array}{rcl}
\displaystyle\bigcup_{i \in I} A_i & = & A_1 \cup A_2
\\
& = & \\{ 1,2,4 \\}
\\
\\
\displaystyle\bigcap_{i \in I} A_i & = & A_1 \cap A_2
\\
& = & \\{ 2 \\}
\end{array}
$$

### Example 2

indexing set:  
$T = \\{ 1,2,3,4 \\}$

indexed family:  
${\cal F} = \\{ A_t \\}_{t \in T} = \\{ A_1,A_2,A_3,A_4 \\}$

_t-th_ term of ${\cal F}$:  
$A_t = \\{ m \in {\Bbb N}: t \lt m \\}$

terms of ${\cal F}$:

$$
\begin{array}{rcl}
A_1 & = & \\{ 2,3,4,5,\dots \\}
\\
A_2 & = & \\{ 3,4,5,6,\dots \\}
\\
A_3 & = & \\{ 4,5,6,7,\dots \\}
\\
A_4 & = & \\{ 5,6,7,8,\dots \\}
\end{array}
$$

generalized union and intersection:

$$
\begin{array}{rcl}
\displaystyle\bigcup_{t \in T} A_t & = & A_1 \cup A_2 \cup A_3 \cup A_4
\\
& = & \\{ 2,3,4,5,\dots \\}
\\
& = & {\Bbb N} \setminus \\{ 1 \\}
\\
\\
\displaystyle\bigcap_{t \in T} A_t & = & A_1 \cap A_2 \cap A_3 \cap A_4
\\
& = & \\{ 5,6,7,8,\dots \\}
\\
& = & {\Bbb N} \setminus \\{ 1,2,3,4 \\}
\end{array}
$$

### Example 3

indexing set:  
$T = \\{ 1,2,3,4 \\}$

indexed family:  
${\cal F} = \\{ A_t \\}_{t \in T} = \\{ A_1,A_2,A_3,A_4 \\}$

_t-th_ term of ${\cal F}$:  
$A_t = \\{ x \in T: x \neq t \\}$

terms of ${\cal F}$:

$$
\begin{array}{rcl}
A_1 & = & \\{ 2,3,4 \\}
\\
A_2 & = & \\{ 1,3,4 \\}
\\
A_3 & = & \\{ 1,2,4 \\}
\\
A_4 & = & \\{ 1,2,3 \\}
\end{array}
$$

generalized union and intersection:

$$
\begin{array}{rcl}
\displaystyle\bigcup_{t \in T} A_t & = & A_1 \cup A_2 \cup A_3 \cup A_4
\\
& = & \\{ 1,2,3,4 \\}
\\
\\
\displaystyle\bigcap_{t \in T} A_t & = & A_1 \cap A_2 \cap A_3 \cap A_4
\\
& = & \varnothing
\end{array}
$$

## Analogy to Sigma/Pi Notation

$\displaystyle\bigcup_{i \in I}$ is similar to $\displaystyle\sum_{i \in I}$, but with terms being sets rather than numbers, and hence with operation $A \cup B$ instead of $A+B$:

$$
\begin{array}{lcl}
\displaystyle\sum_{n \in \Bbb N} n & = &
1+2+3+4+\cdots
\\
\\
\displaystyle\bigcup_{n \in \Bbb N} A_n & = &
A_1 \cup A_2 \cup A_3 \cup A_4 \cup \cdots
\end{array}
$$

the same holds for $\displaystyle\bigcap_{i \in I}$ and $\displaystyle\prod_{i \in I}$ with operation $A \cap B$ instead of $A \cdot B$:

$$
\begin{array}{lcl}
\displaystyle\prod_{n \in \Bbb N} n & = &
1 \cdot 2 \cdot 3 \cdot 4 \cdot \cdots
\\
\\
\displaystyle\bigcap_{n \in \Bbb N} A_n & = &
A_1 \cap A_2 \cap A_3 \cap A_4 \cap \cdots
\end{array}
$$
