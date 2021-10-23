### Algorithms

[Systematic Derivation of Efficient Parallel Algorithms for Generate-test-α Computation](https://www.jstage.jst.go.jp/article/imt/7/2/7_567/_article) (2012)
* Build a linear-time reducer from the semiring operations of the equivalent cubic-time reducer
* Emailed author in March 2021 with link to my [C# code](https://github.com/jasonincanada/kattis/tree/master/cs/semirings) for these ideas (no reply)

[The Yampa arcade](https://dl.acm.org/doi/abs/10.1145/871895.871897) (2003)
* Good intro to functional reactive programming #frp
* Implements a Space Invaders game

[Warm fusion: deriving build-catas from recursive definitions](https://dl.acm.org/doi/abs/10.1145/224164.224223) (1995)
* Uses a rewrite-rule system to fuse `build`/`cata` pairs where they occur in recursive function body expansions


### Databases

[Update semantics of relational views](https://dl.acm.org/doi/10.1145/319628.319634) (1981)
* Classic paper on translating view updates back to their matching updates on the underlying store

[Algebras and update strategies](http://www.jucs.org/jucs_16_5/algebras_and_update_strategies/jucs_16_05_0729_0748_johnson.pdf) (2010)
* Lenses as algebras for a monad in the $Set/V$ category

[Relational Algebra by Way of Adjunctions](http://www.cs.ox.ac.uk/jeremy.gibbons/publications/reladj.pdf) (2018)
* Figure 2 for an overview of the adjunctions underlying relational algebra


### Languages

[Super 8 languages for making movies (functional pearl)](https://dl.acm.org/doi/10.1145/3110274) (2017)
* A language built on Racket for declaratively describing video editing recipes


### Lenses

[What you needa know about Yoneda: profunctor optics and the Yoneda lemma (functional pearl)](https://dl.acm.org/doi/10.1145/3236779) (2018)
* Rendered the derivation of symmetric concrete lenses from p. 84:17 as an orbit diagram
* Rendered the `zipWith3Grate` function from p. 84:23 as an orbit diagram
* #Yoneda lemma

[Traversal Optics and Polynomial Functors.pdf](https://github.com/BartoszMilewski/Publications/blob/master/Traversals.pdf) (2021)
* Van-Laarhoven-style lenses expressed as categorical ends
* Uses #Yoneda lemma twice


### User Interface

[Declarative UIs are the Future — And the Future is Comonadic!](https://functorial.com/the-future-is-comonadic/main.pdf)
* Concise intro to the comonadic structure of UI specifications
