# Operations on Sets

$\large\boldsymbol{A \cup B}$  
every term that belongs to one of sets (or to both)  
$\small\\{ x: x \in A \lor x \in B \\}$

$\large\boldsymbol{A \cap B}$  
every term that belongs both to $A$ and $B$  
$\small\\{ x: x \in A \land x \in B \\}$

$\large\boldsymbol{A \setminus B}\quad$ (or $\large\boldsymbol{A-B}$)  
every term that belongs to $A$ but not to $B$    
$\small\\{ x \in A: x \notin B \\}$

$\large\boldsymbol{A\ {\small\triangle}\ B}$  
every term that belongs to either $A$ or $B$, but not to both (i.e., $(A \setminus B) \cup (B \setminus A)$ )  
$\small\\{ x: (x \in A \land x \notin B) \lor (x \in B \land x \notin A) \\}$

$\large\boldsymbol{A \times B}$  
set of pairs being all possible combinations of $(a \in A, b \in B)$  
$\small\\{ (a,b): a \in A \land b \in B \\}$

$\large\boldsymbol{A^{\complement}}$  
every term from universe $\Bbb{U}$ that does not belong to $A$ (i.e., $\Bbb{U} \setminus A$)  
$\small\\{ x \in {\Bbb U}: A \notin U \\}$

$\large\boldsymbol{{\cal P}(A)}$  
set of all possible subsets of $A$ (including itself and empty set)  
$\small\\{ X: X \subseteq A \\}$

## Examples

### Union, Intersection and Differences

$$
\begin{array}{l}
\\{ 1,2 \\} \cup \\{ 2,3 \\} =
\\{ 1,2,3 \\}
\\
\\{ 1,2 \\} \cap \\{ 2,3 \\} =
\\{ 2 \\}
\\
\\{ 1,2 \\} \setminus \\{ 2,3 \\} =
\\{ 1 \\}
\\
\\{ 1,2 \\} \triangle \\{ 2,3 \\} =
\\{ 1,3 \\}
\end{array}
$$

### Cartesian Product

For $A = \\{1,2 \\}$ and $B = \\{ 2,3 \\}$:

$$
A \times B = \\{
(1,2), (1,3), (2,2), (2,3)
\\}
$$

### Complement

For $A = \\{ 1,2,3 \\}$ in universe $\Bbb{U} = \\{ 1,2,3,4,5 \\}$:

$$
A^{\complement} = {\Bbb U} \setminus A =
\\{ 4,5 \\}
$$

### Power Set

For $A = \\{ 1,2,3 \\}$:

$$
\begin{array}{ll}
{\cal P}(A) = \\{
\\
& \varnothing,
\\
& \\{1\\}, \\{2\\}, \\{3\\},
\\
& \\{1,2\\}, \\{1,3\\}, \\{2,3\\},
\\
& \\{1,2,3\\}
\\
\\}
\end{array}
$$

