# Theorem. In a Hausdorff Space the Intersection of a Set and a Neighbourhood of Its Limit Point Is Infinite

## Theorem

Let $(X, \mathcal T)$ be a [[Definition. Hausdorff space|Hausdorff topological space]]. Let $S \subseteq X$ with $x$ as its [[Definition. Limit Point|limit point]].

Then, for any [[Definition. Neighbourhoods|neighbourhood]] $N$ of $x$, $N \cap S$ is infinite.

## Proof

Aiming for a contradiction, suppose there is a [[Definition. Neighbourhoods|neighbourhood]] $N$ of $x$, such that $N \cap S$ is finite.

By [[Definition. Hausdorff space|Hausdorff property]], for any $s \in N \cap S$, if $s \ne x$, there are [[Definition. Open Sets|open]] $U_s \ni s$, and [[Definition. Open Sets|open]] $V_s \ni x$, such that $U_s \cap V_s = \emptyset$.

Let

$$
V = \bigcap_{s \in N \cap S} V_s.
$$

By [[Definition. Topological Space|Open Set Axiom 3]], $V$ is [[Definition. Open Sets|open]], and

$$
\emptyset = V \cap \left(\bigcup_{s \in N \cap S} U_s \setminus \{x\} \right) \supseteq V \cap (N \setminus \{x\}).
$$

Thus, $x$ is not a [[Definition. Limit Point|limit point]] of $S$, contradicting the condition we have.

$\blacksquare$
