[Explainable dynamic programming](https://doi.org/10.1017/S0956796821000083) #erw21 (2021)

## Value decompositions and sets

Valuation difference between two choices of preference sets $A$ and $B$ (Alice and Bob's rankings of restaurants, etc):

$$\delta(A,B) = \{(c, x-y) | (c,x) \in \varphi(A), (c,y) \in \varphi(B)\}$$

The negative components ($x - y < 0$) of the difference are called its *barrier*:

$$\delta^{-}(A,B) = \{ (c,x) | (c,x) \in \delta(A,B), x < 0\}$$

The *dominator components* are the positive components $\delta^{+}(A,B)$ with $x > 0$.

Any subset $d$ of $\delta^{+}(A,B)$ whose total $\overset{\textasciicircum}{d}$ (sum of components $x$) is larger than the whole barrier $\vert\overset{\textasciicircum}{\delta^{-}}(A,B)\vert$ is a *dominator*.  The set of all dominators is:

$$\Delta(A,B) = \{D \vert D \subseteq \delta^{+}(A,B), \overset{\textasciicircum}{D} > \vert\overset{\textasciicircum}{\delta^{-}}(A,B)\vert \}$$

Minimal dominating set, a "quickest" explanation (by smallest set cardinality, not element values) for why the barrier was overcome by support p.7:

$$\underline{\Delta} = \{D | D \in \Delta(A,B), \forall D' \in D. D' \notin \Delta(A,B) \}$$


## Semirings

![[erw21 fig 4 - semiring axioms.png]]

"Along with the semiring recurrence representation, one also needs to know the semiring over which this representation is defined. In the case of Fibonacci, it is the `Counting` semiring. The semiring recurrence representation and the semiring over which it is defined determine the computation they represent." p. 9


## View Semiring

The `View` semiring lets us describe the components of an optimal solution instead of just what the optimal value is

![[erw21 - view semiring.png]]

**Echoes of the past:** The [Linear A script](https://en.wikipedia.org/wiki/Linear_A), used on Crete by the Minoans from 1800 - 1450 BC, is still largely undeciphered, but we have some idea of their use of numbers in practice. In particular, from the [Unicode script proposal for Linear A](https://www.unicode.org/L2/L2010/10422-n3973-lineara.pdf), p. 3:

    "Unlike Linear B, which has a complex system for recording the weights and volumes of dry and liquid commodities separately, Linear A does not; it merely records amounts, it being up to the reader to assume individual units (e.g., people or animals) or dry or liquid measurements according to the commodity"


## Minimal Dominators and Explanations

![[erw21 fig 8 - minimal dominators explanations.png]]

![[erw21 - explainWith.png]]


## General Workflow

Copied from p. 18:

"The generation of explanation works in much the same way for other DP algorithms. The general workflow is as follows.
- Identify the appropriate semiring for the optimization problem. This might require the definition of a new Haskell data type and its `Semiring` instance. The `View` semiring offers opportunities to realize a variety of computations that produce results on different levels of detail.
- Implement the DP algorithm as a type class that contains the main recurrence, a wrapper to run the described computation, plus the function `result` that ties the DP computation to different result types.
- Define a value decomposition for the result type. The categorization of the type of values to be optimized allows the function `explainWith` to compare optimal results with alternatives and produce explanations based on value categories"


## Examples

### Shortest Path

![[erw21 - spa recurrence relation.png]]

![[erw21 fig 5 - generic spa.png]]

### Knapsack

![[erw21 fig 9 - knapsack dp.png]]

### Viterbi

Hidden Markov Models - infer a sequence of hidden states from visible observations

See [[Bayes Theorem and Viterbi]]

![[erw21 fig 10 - viterbi dp.png]]
