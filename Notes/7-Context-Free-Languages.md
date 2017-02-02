# Context Free Languages

## Context Free Grammars

**Context free grammars (CFGs)** use variables to represent strings of symbols, called *terminals*. Each variable has a collection of rules determining the strings it can represent.

**Example**

Consider the context free grammar, $G$, which has the following substitution rules

\begin{aligned}
    A &\to 0 A 1 \newline
    A &\to B \newline
    B &\to #. \newline
\end{aligned}

If we take the start variable (the first $A$) and repeatedly substitute in the variables (in no particular scheme) then we get one of the **derivations** of the grammar. For Example

$$
  000#111.
$$
