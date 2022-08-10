# Theorem. Compact Subspaces of Hausdorff Spaces Are Closed

## Theorem

Let $X$ be a be a [[Definition. Hausdorff space|Hausdorff space]]. Let $S$ be a [[Definition. Subspaces|subspace]] of $X$.
	
Then, if $S$ is [[Definition. Compact Spaces|compact]] in $X$, then $S$ is [[Definition. Closed Sets|closed]] in $X$.

## Proof

If $S$ is [[Definition. Closed Sets|closed]] in $X$, then $X \setminus S$ is [[Definition. Open Sets|open]]. Thus, we need to show that $X \setminus S$ is [[Definition. Open Sets|open]] in $X$.

Let $x \in X \setminus S$ be arbitrary.

As $X$ is [[Definition. Hausdorff space|Hausdorff]], $S$ is also [[Definition. Hausdorff space|Hausdorff]]. Thus, for any $s \in S$, there exist [[Definition. Neighbourhoods|open neighbourhoods]] $U_s$ and $V_s$ with $s \in U_s$ and $x \in V_s$, such that $U_s \cap V_s$ is empty.

As $\displaystyle S \subseteq \bigcup_{s \in S} U_s$ and every $U_s$ is [[Definition. Open Sets|Open]], $\{U_s : s \in S\}$ is an [[Definition. Cover|open cover]] of $S$.

As $S$ is [[Definition. Compact Spaces|compact]], there is a finite $F \subseteq S$, such that $\{U_s : s \in F\}$ is a finite [[Definition. Subcovers|subcover]] of $S$.

In this case, there are finitely many [[Definition. Neighbourhoods|open neighbourhood]] $V_s$ of $x$, such that for any $s \in F$, $U_s \cap V_s = \emptyset$.

Let

$$
V = \bigcap_{s \in F} V_s.
$$

By [[Definition. Topological Space|Open Set Axiom 3]], $V$ is [[Definition. Open Sets|open]].

As

$$
\emptyset = V \cap \bigcup_{s \in F} U_s \supseteq S,
$$

$V$ is the required [[Definition. Neighbourhoods|open neighbourhood]] of $x$, such that $V_a \cap S = \emptyset$, i.e., $V_a \subseteq X \setminus S$.

As $x$ is arbitrary, $X \setminus S$ is [[Definition. Open Sets|open]]. #why

$\blacksquare$

## Remark

In this proof, note that every [[Definition. Neighbourhoods|open neighbourhood]] $V_s$ of $x$ is depend on the [[Definition. Neighbourhoods|open neighbourhood]] $U_s$ of $s$. In this case, $\{V_s:s \in S\}$ is not necessarily finite. If $\{V_s : s \in S\}$ is infinite, there is no reason to find a "minimum" $V_s$ such that it disjoints $S$. That is why the proof can not be done here.

For example, [[Definition. Euclidian Space|Euclidian space]] $\mathbb R$ is [[Definition. Hausdorff space|Hausdorff]] as [[Theorem. Metric Spaces are Hausdorff|metric spaces are Hausdoff]]. For any $x \in [0,1)$, we can find [[Definition. Neighbourhoods|open neighbourhoods]] $U_x$ of $x$ and $V_x$ of $1$, such that $U_x \cap V_x$ is empty, but $[0,1)$ is not [[Definition. Open Sets|open]] in $\mathbb R$.