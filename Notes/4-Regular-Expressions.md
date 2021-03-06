# Regular Expressions

We can use regular operations to build up **regular expressions** which describe languages.

For example,

$$
  (a \cup b)a^*
$$

is an $a$ or a $b$ followed by zero or more $a$'s.

## Formal Definition

We say $R$ is a **regular expression** if $R$ is

1. $a$ for some $a$ in the alphabet $\Sigma$,
2. $\varepsilon$,
3. $\varnothing$,
4. $(R_1 \cup R_2)$, where $R_1$ and $R_2$ are regular expressions,
5. $(R_1 \circ R_2)$, where $R_1$ and $R_2$ are regular expressions, or
6. $(R)^*$, where $R$ is a regular expression.

Note that $\varepsilon$ is a language with only one string, the empty string ($\epsilon$), and $\varnothing$ is the language with no strings.

## Regular Expressions and Languages

### Theorem

A language is regular if and only if some regular expression describes it.

#### Proof

**Base**: 

$R$ | $L(R)$ | $M$[^1]
:-:|:-:|:-:
$\varnothing$ | $\varnothing$ | ![]()
$\varepsilon$ | $\{\varepsilon\}$ | ![]()
$a$ | $\{a\}$ | ![]()

[^1]: $L(R) = L(M)$

## Nondeterminate Finite Automata to Regular Expressions


Given any nondeterminate finite automata we can construct an eqivalent nondeterminate finite automata with

1. exactly one accept state,
2. no arrows to the start state,
3. no arrows out of the accept state, and
4. the accept state is not the start state.
