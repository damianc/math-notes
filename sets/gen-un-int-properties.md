# Properties of Generalized Unions and Intersections

$$
A_t \subset \bigcup_{t \in T} A_t
$$

$$
A_t \supset \bigcap_{t \in T} A_t
$$

$$
\underset{t \in T}{\Large\forall} A_t \subset A
\leadsto
\bigcup_{t \in T} A_t \subset A
$$

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


