[Exploiting the Commutativity Lattice](https://dl.acm.org/doi/abs/10.1145/1993498.1993562) (2011) #kul11

Introduces the *commutativity lattice* for reasoning about which operations on a data structure can be parallelized.  The task for the developer is to consider every pair of methods on the structure and precisely denote their commutativity conditions

## Sets

For instance, the operations on sets, `add()`, `remove()`, and `contains()`:

![[kul11 - commutativity spec for sets.png]]

In the notation

$$\langle\text{add}(a)\rangle_{\sigma_1}/r_1,$$

$\sigma_1$ is the starting state (set) for the operation add($a$), and $r_1$ is the return value, a boolean denoting whether the underlying state was actually modified.  The above adds $a$ to the set $\sigma_1$, and returns $r_1$.  Rule (1) in Figure 2 states that two add() operations commute if their arguments $a$ and $b$ are different, or if both operations have no effect on the set (the element is already a member)


## $k$-d trees

The commutativity spec for [$k$-d trees](https://en.wikipedia.org/wiki/K-d_tree):

![[kul11 - commutativity spec kd trees.png]]

Rule (2) in Figure 4 states that `nearest(a)` commutes with `add(b)` if $r_2$ is false (the element $b$ was already a member so its addition had no effect on the tree) or if the distance between $a$ and $b$ is greater than the distance between $a$ and `nearest(a)`, meaning the added element $b$ would have no effect on the return $r_1$ from `nearest(a)`--there's already something closer to $a$ than $b$


## Union find

The commutativity spec for the *union find* operation:

![[kul11 - commutativity spec union find.png]]

## 2.4 A Commutativity Lattice

From p. 4:

> While the lattice has been defined only for a pair of methods of an ADT, it can be readily extended to create a bounded lattice of commutativity specifications, with elements of the lattice representing specifications that are distinct up to logical equivalence. For two commutativity specifications $\Phi_1$ and $\Phi_2$, $\Phi_1 \preceq \Phi_2$ if and only if, for each pair of methods $m_1$, $m_2$, where $\phi_1$ is the commutativity condition for $m_1$ and $m_2$ from $\Phi_1$, and $\phi_2$ is the corresponding condition from $\Phi_2$, $\phi_1 \preceq \phi_2$.

> We can define $\sqcap$ and $\sqcup$ in a similar manner (joining or meeting corresponding pairs of commutativity conditions from the two specifications). $\perp$ is the specification where all conditions are **false**, and $\top$ is the specification where all conditions are precise: $\Phi^∗$

---

## CUE lang

See also: [CUE - What is a lattice?](https://cuelang.org/docs/concepts/logic/#what-is-a-lattice)

![[cue lang - lattice example.png]]

An example lattice from the CUE website
