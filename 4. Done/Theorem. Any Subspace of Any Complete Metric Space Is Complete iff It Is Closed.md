# Theorem. Any Subspace of Any Complete Metric Space Is Complete iff It Is Closed

## Theorem

Let $(X, \rho)$ be a [[Definition - Complete Metric Spaces|complete]] [[Definition. Metric Spaces|metric space]].

Let $(S, \rho')$ be a [[Definition. Subspaces|subspace]] of $(X, \rho)$.

$(S, \rho')$ is [[Definition - Complete Metric Spaces|complete]] iff $S$ is [[Definition. Closed Sets|closed]] in $(X, \rho)$.

## Proof

Aiming for a contradiction, suppose $(S, \rho')$ is [[Definition. Compact Spaces|complete]] but $S$ is not [[Definition. Closed Sets|closed]].

As $S$ is not [[Definition. Closed Sets|closed]], there is an $x \in X \setminus S$ which is a [[Definition. Limit Point|limit point]] of $S$.

Bu [[Theorem. In a Hausdorff Space the Intersection of a Set and a Neighbourhood of Its Limit Point Is Infinite]], for any $\delta \in \mathbb R_{> 0}$, the [[Definition. Balls|open ball]] $B(x, \delta) \cap S$ must be infinite.

Let $r \in \mathbb R_{> 0}$. Let $p \in S$.

For any $n \in \mathbb N$, let $s_n$ be a member in $B(s, r^{-n}) \setminus B(s, r^{-(n + 1)})$ if this complement is not empty; if it is empty, then, let $s_n = p$. Then, we have $\langle s_n \rangle_{n \in \mathbb N}$ as a sequence [[Definition. Convergent Sequences|converging]] to $x$.

By [[Theorem. Convergent Sequence is Cauchy]] $\langle s_n \rangle_{n \in \mathbb N}$ is [[Definition. Cauchy Sequences|Cauchy]].

By [[Theorem. Convergent Sequences Are Closed in Hausdorff Space]], for any $I \subseteq \mathbb N$, $\{s_n\}_{n \in I}$ is [[Definition. Closed Sets|closed]] in $(X, \rho)$.

Thus, for any $m \in \mathbb N$, $X \setminus \{s_n : n > m\}$ is [[Definition. Open Sets|open]]. #why 

Let

$$
\mathcal U = \left\{ X \setminus \{s_n : n > m\} : m \in \mathbb N \right\},
$$

then $\mathcal U$ is an [[Definition. Cover|open cover]] of $S$. But, as for any $m \in \mathbb N$,

$$
\bigcup_{m \in \mathbb N} \{X \setminus \{s_n : n > m\}\} \subsetneq S,
$$

$\mathcal U$ has no [[Definition. Subcovers|subcover]] for $S$.

This implies that $(S, \rho')$ is not [[Definition - Complete Metric Spaces|complete]], contradicting the condition we have.

$\blacksquare$

