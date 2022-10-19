# The Boolean Algebra of Sets
It is clear that set theory is closely related to logic. The intersection and union of sets can be defined in terms of the logical ‘and’ and logical ‘or’ operators. The notation $\{x | P(x)\}$ makes it possible to use predicates to specify sets. And if *A* is any set, then the formula $x \in A$ defines a one place predicate that is true for an entity *x* if and only if *x* is a member of *A*. So it should not be a surprise that many of the rules of logic have analogues in set theory.

For example, we have already noted that $\cup$ and $\cap$ are commutative operations. This fact can be verified using the rules of logic. Let *A* and *B* be sets. According to the definition of equality of sets, we can show that $A \cup B = B \cup A$ by showing that $\forall x((x \in A \cup B) \leftrightarrow (x \in B \cup A))$. But for any *x*,
$$
\begin{align}
x \in A \cup B \leftrightarrow x \in A \vee x \in B \\ 
\leftrightarrow x \in B \vee x \in A \\
\leftrightarrow x \in B \cup A\ \ \ \ \ \ \
\end{align}
$$
The commutativity of $\cap$ follows in the same way from the definition of $\cap$ in terms of $\wedge$ and the commutativity of $\wedge$, and a similar argument shows that union and intersection are associative operations.

The distributive laws for propositional logic give rise to two similar rules in set theory. Let *A*, *B*, and *C* be any sets. Then
$$
A \cup (B \cap C) = (A \cup B) \cap (A \cup C)
$$
and
$$
A \cap (B \cup C) = (A \cap B) \cup (A \cap C)
$$
These rules are called the **distributive laws** for set theory. To verify the first of these laws, we just have to note that for any *x*,
$$
\begin{align}
x \in A \cup (B \cap C) \\
\leftrightarrow (x \in A) \vee ((x \in B) \wedge (x \in C)) \\
\leftrightarrow ((x \in A) \vee (x \in B)) \wedge ((x \in A) \vee (x \in C)) \\
\leftrightarrow (x \in A \cup B) \wedge (x \in A \cup C) \\
\leftrightarrow x \in ((A \cup B) \cap (A \cup C)) \\
\end{align}
$$
The second distributive law for sets follows in exactly the same way.

## Index
- [[1. Set complement]]
- [[2. Link between logic and set theory]]