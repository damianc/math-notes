# Indexed Family of Sets

- **family of sets** is a set that consists of sets, for example:

$$
{\cal F} = \\{ \\{1,2\\}, \\{2,4\\}\\}
$$

- **indexed family of sets** is a set of sets referenced by some index (being a term of **indexing set**), for example, if _indexing set_ $I = \\{ 1,2 \\}$:

$$
{\cal F} = \\{ A_i \\}_{i \in I} =
\\{ A_i\ |\ i \in I \\} = \\{ A_1, A_2 \\}
$$

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
\begin{array}{ccl}
A_1 & = & \\{ 1,2 \\}
\\
A_2 & = & \\{ 2,4 \\}
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
\begin{array}{ccl}
A_1 & = & \\{ m \in {\Bbb N}: 1 \lt m \\}
\\
& = & \\{ 2,3,4,5,\dots \\}
\\
A_2 & = & \\{ m \in {\Bbb N}: 2 \lt m \\}
\\
& = & \\{ 3,4,5,6,\dots \\}
\\
A_3 & = & \\{ m \in {\Bbb N}: 3 \lt m \\}
\\
& = & \\{ 4,5,6,7,\dots \\}
\\
A_4 & = & \\{ m \in {\Bbb N}: 4 \lt m \\}
\\
& = & \\{ 5,6,7,8,\dots \\}
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
\begin{array}{ccl}
A_1 & = & \\{ x \in T: x \neq 1 \\}
\\
& = & \\{ 2,3,4 \\}
\\
A_2 & = & \\{ x \in T: x \neq 2 \\}
\\
& = & \\{ 1,3,4 \\}
\\
A_3 & = & \\{ x \in T: x \neq 3 \\}
\\
& = & \\{ 1,2,4 \\}
\\
A_4 & = & \\{ x \in T: x \neq 4 \\}
\\
& = & \\{ 1,2,3 \\}
\end{array}
$$

### Example 4

indexing set:  
$T = {\Bbb N}$

indexed family:  
${\cal F} = \\{ A_n \\}\_{n \in T} = \\{ A_1,A_2,A_3,A_4,\dots \\}$

_n-th_ term of ${\cal F}$:  
$A_n = \\{ x \in {\Bbb Z}: (-1)^n \le x \le n \\}$

first 4 terms of ${\cal F}$:

$$
\begin{array}{ccl}
A_1 & = &  \\{ x \in {\Bbb Z}: -1 \le x \le 1 \\}
\\
& = & \\{ -1,0,1 \\}
\\
A_2 & = &  \\{ x \in {\Bbb Z}: 1 \le x \le 2 \\}
\\
& = & \\{ 1,2 \\}
\\
A_3 & = &  \\{ x \in {\Bbb Z}: -1 \le x \le 3 \\}
\\
& = & \\{ -1,0,1,2,3 \\}
\\
A_4 & = &  \\{ x \in {\Bbb Z}: 1 \le x \le 4 \\}
\\
& = & \\{ 1,2,3,4 \\}
\end{array}
$$

$$
\cdots \cdots \cdots \cdots
$$

### Example 5

> index is not required to be a natural number; index $i$ can belong to any set, for example ${\Bbb Z}$ or ${\Bbb R}$, and therefore be assigned value like $-\sqrt{2}$ or $\frac{1}{2}$

indexing set:  
$K = {\Bbb Z}$

indexed family:  
${\cal F} = \\{ A_k \\}\_{k \in K} = \\{ \dots,A_{-1},A_0,A_1,A_2,\dots \\}$

_k-th_ term of ${\cal F}$:  
$A_k = \\{ x \in {\Bbb Z}: |x| \le k^2 \\}$

example terms of ${\cal F}$:

$$
\cdots \cdots \cdots \cdots
$$

$$
\begin{array}{ccl}
A_{-1} & = &  \\{ x \in {\Bbb Z}: |x| \le 1 \\}
\\
& = & \\{ -1,0,1 \\}
\\
A_0 & = &  \\{ x \in {\Bbb Z}: |x| \le 0 \\}
\\
& = & \\{ 0 \\}
\\
A_1 & = &  \\{ x \in {\Bbb Z}: |x| \le 1 \\}
\\
& = & \\{ -1,0,1 \\}
\\
A_2 & = &  \\{ x \in {\Bbb Z}: |x| \le 4 \\}
\\
& = & \\{ -4,-3,-2,-1,0,1,2,3,4 \\}
\end{array}
$$

$$
\cdots \cdots \cdots \cdots
$$
