# Alphabets and Languages

**Lecture 1 - January 5, 2017**

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

_definition_: A **language** is a set of strings over an alphabet. We can apply set opertations like,

* Union
* Intersection
* Set Difference.

Given a language $A$, the **complement** of $A$, denoted $\bar A$, is

$$
    \bar A = \Sigma - A.
$$



