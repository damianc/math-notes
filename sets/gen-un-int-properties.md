# Properties of Generalized Unions and Intersections

## Membership

- $x$ belongs to a union if it is present in _at least one subset_ of a family:

$$
\left( x \in \bigcup_{t \in T} A_t \right)
\iff
\underset{t \in T}{\large\exists}
\left( x \in A_t \right)
$$

- $x$ does not belong to a union if there is _no subset_ that contains it:

$$
\left( x \notin \bigcup_{t \in T} A_t \right)\iff\underset{t \in T}{\large\forall}\left( x \notin A_t \right)
$$

- $x$ belongs to an intersection if it is present in _every subset_ of the family:

$$
\left( x \in \bigcap_{t \in T} A_t \right)
\iff
\underset{t \in T}{\large\forall}
\left( x \in A_t \right)
$$

- $x$ does not belong to an intersection if there is _at least one subset_ that does not contain it:

$$
\left( x \notin \bigcap_{t \in T} A_t \right)
\iff
\underset{t \in T}{\large\exists}
\left( x \notin A_t \right)
$$

## Subsets and Supersets

- every term of a family is a subset of the union:

$$
A_t \subset \bigcup_{t \in T} A_t
$$

- every term of a family is a superset of the intersection:

$$
A_t \supset \bigcap_{t \in T} A_t
$$

- if every term of a family is a subset of $A$, the union is a subset of $A$:

$$
\underset{t \in T}{\Large\forall} A_t \subset A
\leadsto
\bigcup_{t \in T} A_t \subset A
$$

- if every term of a family is a superset of $A$, the intersection is a superset of $A$:

$$
\underset{t \in T}{\Large\forall} A_t \supset A
\leadsto
\bigcap_{t \in T} A_t \supset A
$$

----

$$
\begin{array}{l}
\left|\begin{array}{l}
A \cup \left[\displaystyle\bigcup_{t \in T} A_t \right] \quad=\quad
\displaystyle\bigcup_{t \in T}\  (A \cup A_t)
\\
\ 
\\
\left[\displaystyle\bigcup_{t \in T} A_t \right] \cup \left[\displaystyle\bigcup_{t \in T} B_t \right] \quad=\quad
\displaystyle\bigcup_{t \in T}\  (A_t \cup B_t)
\end{array}\right.
\\
\ 
\\
\ 
\\
\left|\begin{array}{l}
A \cap \left[\displaystyle\bigcap_{t \in T} A_t \right] \quad=\quad
\displaystyle\bigcap_{t \in T}\  (A \cap A_t)
\\
\ 
\\
\left[\displaystyle\bigcap_{t \in T} A_t \right] \cap \left[\displaystyle\bigcap_{t \in T} B_t \right] \quad=\quad
\displaystyle\bigcap_{t \in T} \ (A_t \cap B_t)
\end{array}\right.
\\
\ 
\\
\ 
\\
\left|\begin{array}{l}
A \cup \left[\displaystyle\bigcap_{t \in T} A_t \right] \quad=\quad
\displaystyle\bigcap_{t \in T}\  (A \cup A_t)
\\
\ 
\\
\left[\displaystyle\bigcap_{t \in T} A_t \right] \cup \left[\displaystyle\bigcap_{t \in T} B_t \right] \quad{\boldsymbol{\large\subset}}\quad
\displaystyle\bigcap_{t \in T} \ (A_t \cup B_t)
\end{array}\right.
\\
\ 
\\
\ 
\\
\left|\begin{array}{l}
A \cap \left[ \displaystyle\bigcup_{t \in T} A_t \right] \quad=\quad
\displaystyle\bigcup_{t \in T} \ (A \cap A_t)
\\
\ 
\\
\left[\displaystyle\bigcup_{t \in T} A_t \right] \cap \left[\displaystyle\bigcup_{t \in T} B_t \right] \quad{\boldsymbol{\large\supset}}\quad
\displaystyle\bigcup_{t \in T} \ (A_t \cap B_t)
\end{array}\right.
\end{array}
$$

----

$$
\begin{array}{l}
\left|\begin{array}{l}
A - \displaystyle\bigcup_{t \in T} A_t =
\displaystyle\bigcap_{t \in T}\ (A-A_t)
\\
\ 
\\
A - \displaystyle\bigcap_{t \in T} A_t =
\displaystyle\bigcup_{t \in T}\ (A-A_t)
\end{array}\right.
\\
\ 
\\
\ 
\\
\left|\begin{array}{l}
X - \displaystyle\bigcup_{t \in T} A_t =
\displaystyle\bigcap_{t \in T}\ (X-A_t)
\\
\ 
\\
X - \displaystyle\bigcap_{t \in T} A_t =
\displaystyle\bigcup_{t \in T}\ (X-A_t)
\end{array}\right.
\\
\ 
\\
\ 
\\
\left|\begin{array}{l}
\ - \displaystyle\bigcup_{t \in T} A_t =
\displaystyle\bigcap_{t \in T}\ -A_t
\\
\ 
\\
\ - \displaystyle\bigcap_{t \in T} A_t =
\displaystyle\bigcup_{t \in T}\ -A_t
\end{array}\right.
\end{array}
$$


