# Minimizing Discreet Finite Automata

Given a discreet finite automaton, $M = (Q, \Sigma, \delta, q_0, F)$, for a language $L$, we canstruct a **minimal** discreet finite automaton with as few states as possible. This discreet finite automaton is isomorphically unique.

## Process

Given $M = (Q, \Sigma, \delta, q_0, F)$, and $q \in Q$, let $M_q$ be identical to $M$, but with state $q$ instead of $q_0$.

Then $p$ and $q$ can be collapse if $L(M_p) = L(M_q)$.

Consider $M$ with $p$ and $q$ collapsed to $pq$, let's call this $M^\prime$.


