# Alphabets and Languages

## Strings and Symbols

_definitions_:

* An **alphabet** is a finite set of set of symbols, we denote an arbitrary alphabet $\Sigma$.
* A **string** is a finite sequence of symbols from the alphabet.
* The **empty string** is the string with no symbols denoted $\epsilon$.

### Operations and Relations on Strings

#### Concatenation

Given two strings $x$ and $y$ the **concatenation** of $x$ and $y$ denoted $xy$ is the the two string combined end-to-end.

Concatenation is associative, so $xyz = (xy)z = x(yz)$.

We let $x^n$ be $x$ concatenated with itself $n$ times.

#### Substrings

A string $v$ is a **substring** of $w$ if and only if there exist strings $x$ and $y$ such that

$$
    W = xvy,
$$

If $x = \epsilon$ then $v$ is a **prefix** of $w$, if $y = \epsilon$ then $v$ is a **suffix** of $w$.

#### Reversal

Give a string $w$, the **reversal** of $w$ is denoted $w^R$.

## Languages

**Lecture 2 - January 9, 2017**

_definition_: A **language** is a set of strings over an alphabet. We can apply set opertations like,

* Union
* Intersection
* Set Difference.

Given a language $A$, the **complement** of $A$, denoted $\bar A$, is

$$
    \bar A = \Sigma - A.
$$

Given languages $L_1$ and $L_2$ over $\Sigma$, their **concatenation** is,

$$\begin{aligned}
    L = L_1 \cdot L_2 = \{w \in \Sigma^* : w = xy; x \in L_1, y \in L_2 \}.
\end{aligned}$$

Sometime we denote $L_1 \cdot L_2$ as $L_1 L_2$.

### Kleene star

_definition_: The **Kleene star** of a language $L$, denoted $L^*$ is the set of all strings obtained by concatenating more or more strings from $L$, i.e.,

$$\begin{aligned}
    L^* = \{w \in \Sigma^* : w = w_1 w_2 \ldots w_k; k \ge 0, w_i \in L \}.
\end{aligned}$$

For example, the star of $\Sigma$ is $\Sigma^*$, the star of $\varnothing$ is ${\epsilon}$.

## Problems

### Decision vs Search

* **Decision**: Given a formula $\varphi(x_1,x_2,\ldots)$ is there a setting of variables such that $\varphi = T$.
* **Search**: Given $\varphi$, return a satisfying assignment if one exists.

Some examples,

* *Is a graph 3-colourable?* is a **decision** problem.
* *What is a  3-colouring of this graph?* is a **search** problem.


