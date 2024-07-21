# Pascal's Triangle

$$
\tiny
\begin{array}{cccccccccccc}
&&&&&& 1 &&&&&& \\
&&&&& 1 && 1 &&&&& \\
&&&& 1 && 2 && 1 &&&& \\
&&& 1 && 3 && 3 && 1 &&& \\
&& 1 && 4 && 6 && 4 && 1 && \\
& 1 && 5 && 10 && 10 && 5 && 1 & \\
1 && 6 && 15 && 20 && 15 && 6 && 1 \\
...&...&...&...&...&...&...&...&...&...&...&...&...
\end{array}
$$

- with __binomial coefficients__:

$$
\tiny
\begin{array}{cccccccccccc}
&&&&&& \binom{0}{0} &&&&&& \\
&&&&& \binom{1}{0} && \binom{1}{1} &&&&& \\
&&&& \binom{2}{0} && \binom{2}{1} && \binom{2}{2} &&&& \\
&&& \binom{3}{0} && \binom{3}{1} && \binom{3}{2} && \binom{3}{3} &&& \\
&& \binom{4}{0} && \binom{4}{1} && \binom{4}{2} && \binom{4}{3} && \binom{4}{4}
\\
&...&...&...&...&...&...&...&...&...&...&...
\end{array}
$$

## Terms of n-th Row

A set of terms of n-th row of Pascal's triangle can be defined with set-builder notation as follows:

$$
\left\\{
t_i \ |\ i \in [0,n],
t_i = \binom{n}{i}
\right\\}
$$
