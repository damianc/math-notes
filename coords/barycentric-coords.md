# Barycentric Coordinates

Is a point $P$ within a triangle $\triangle_{ABC}$?

**SOLUTION**

$$
\begin{array}{l}
\Delta = (y_B-y_C)(x_A-x_C)+(x_C-x_B)(y_A-y_C)
\\
\Lambda(v,h) = v(x_P-x_C) + h(y_P-y_C)
\\
\\
\lambda_1 = \frac{1}{\Delta}[\Lambda(y_B-y_C,x_C-x_B)]
\\
\lambda_2 = \frac{1}{\Delta}[\Lambda(y_C-y_A,x_A-x_C)]
\\
\lambda_3 = 1 - \lambda_1 - \lambda_2
\\
\\
P \text{ is within } \triangle_{ABC} \text{ if}:
\\
\quad
\underset{i\in\langle1,3\rangle}{\large\forall}
\lambda_i \in \langle0,1\rangle
{\ }\cap{\ }
\lambda_1\lambda_2\lambda_3 \neq 0
\\
\\
P \text{ is on edge of } \triangle_{ABC} \text{ if}:
\\
\quad
\underset{i\in\langle1,3\rangle}{\large\forall}
\lambda_i \in \langle0,1\rangle
{\ }\cap{\ } 
\lambda_1\lambda_2\lambda_3 = 0
\\
\\
P \text{ is beyond } \triangle_{ABC} \text{ if}:
\\
\quad
\underset{i\in\langle1,3\rangle}{\large\exists}
\lambda_i \notin \langle0,1\rangle
\end{array}
$$
