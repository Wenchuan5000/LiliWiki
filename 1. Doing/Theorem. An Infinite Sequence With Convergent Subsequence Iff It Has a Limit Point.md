# Theorem. An Infinite Sequence With Convergent Subsequence Iff It Has a Limit Point

Let $(X, \mathcal T)$ be a [[Definition. Topological Space|topological space]]. Let $u: \mathbb N \to X$ be a sequence satisfying the following conditions:

1. $u[\mathbb N]$ is infinite;

2. There is a subsequence $w$ of $u$ such that $w$ is convergent to a point $l \in X$.

Then, there is at least one $n \in \mathbb N$, such that $u(n)$ is a [[Definition. Limit Point|limit point]] of $u[\mathbb N]$.

## Proof

Aiming for a contradiction, suppose $u[\mathbb N]$ has no [[Definition. Limit Point|limit points]].

Then, for any $n \in \mathbb N$, there is a [[Definition. Neighbourhoods|open neighbourhood]] $U_n$ of $u(n)$, such that

$$
u[\mathbb N] \cap (U_n \setminus \{ u(n) \}) = \emptyset.
$$

