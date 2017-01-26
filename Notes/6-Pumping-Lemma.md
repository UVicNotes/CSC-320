# The Pumping Lemma

Consider

$$
  L = \{ a^n b^n |n \ge 0 \}
$$

Intuitively: we must remember how far the center point is from the start to accept the string. But finite automata have only finite memory, and the center can be arbitrarily far from the start.

**Proof $L$ is non-regular**

Suppose to the contrary that $L$ is regular. Then there exists a discrete finite automaton $M$ such that $L = L(M)$. Let $s$ denote the number of states in $M$.

Given $a^n b^n$ for $n > s$, by the pigeon hole principal ([&icon-wikipedia;](https://en.wikipedia.org/wiki/Pigeonhole_principle)), $M$ must be in some state more than once, say state $p$.

Partition $a^n b^n$ into three strings, $x_\text{before}, x, x_{after}$, divided on the two times we enter state $p$. Let $i = |x|$ be the length of the string of the middle string, $x$, between the two $p$'s.

$$
  \underbrace{aaa \ldots aa}_{x_\text{before}} \underbrace{abb\ldots bb}_{x} \underbrace{b \ldots bbb}_{x_\text{after}}
$$

We can skip this string $x$ or repeat it any number of times and be in the same state ($p$). Thus for any $k \ge 0$, $a^{n+(k-1)i}b^n \in L(M)!$, i.e., $a^{n-i}b^n \in L(M)$ so $a^{n-i}b^n = a^nb^n$. But $i \neq 0$, a contradiction.

