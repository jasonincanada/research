[Functorial Dynamics and Interaction: A computational design environment](http://www.dspivak.net/grants/AFOSR2020-Topos-ContextDependence.pdf)
* [Spivak](http://www.dspivak.net/)'s proposal for research on $Poly$ and its applications
* Another intro to $Poly$ basics
* [Idris code](https://github.com/ToposInstitute/poly/blob/main/code-examples/poly_up_to_fibonacci.idr)

p. 6:

> Arenas and the models that connect them form a mathematical *category*. Its objects are arenas, and its morphisms are models. It turns out that this category is equivalent to a well-known category, that of polynomial functors; which we denote $Poly$. In a surprising way, the simplest polynomials from algebra class encode (the simplest) arenas. To see this, take any polynomial, e.g. $P(y) = y^2 + 2y + 1$, and write it out as a sum $\sum y^i$ of pure-power terms:

$$P(y) = y^2 + y^1 + y^1 + y^0$$

> As an arena, the four summands refer to four positions; in the first position there are two available distinctions, in the second and third positions there is only one available distinction, and in the fourth there are none. But these are only the simplest polynomials; in dependent type theory we can be much more general, as one can see in the following Idris code:

```idris
record Arena where
   constructor MkArena             -- To construct an arena, define:
   position    : Type              -- the meaning of "positions", and
   distinction : position -> Type  -- the meaning of "distinctions".
```

> This syntax says that one can choose any type to serve as the positions: one is not limited to the four element set as above, but instead could use the type **Double** of double-precision floating point numbers for encoding the real numbers $\mathbb{R}$. Similarly one could define the type of positions to be $\mathbb{R}^n$ (**Vect n Double**) for any $n : \mathbb{N}$, but also much more generally one can use **Arena : Type** as its positions. It is as easy to express a machine that spits out arenas as a machine that spits out Doubles.

p. 7:

```idris
Lineland : Arena
Lineland = MkArena Double dis --In Lineland positions are real numbers.
   where
      dis : Double -> Type    --The distinctions may vary by location:
      dis x = if x < 0               --At negative x's,
              then Double            --we can only hear; otherwise,
              else (Double, Double)  --we can both see and hear.
```

>The above Idris code is perfectly good as mathematical syntax, though a more traditional polynomial form for the arena called Lineland would be:

![[poly - lineland.png]]

> The morphisms in $Poly$ are what we called models at the start of Section 1.1. Mathematically, they are precisely the *natural transformations* between polynomial functors. But here is an equivalent definition that fits our informal description above.

```idris
record Model (internal : Arena) (external : Arena) where
   constructor MkModel
   steer : position internal -> position external
   watch : (p : position internal) ->
                distinction external (steer p) ->
                distinction internal p
```

Footnote from p. 6:

> We use the variable $y$ because it stands for Yoneda; indeed, the fundamental category theoretic result known as the Yoneda lemma is involved when one regards the polynomial $y^2 + 2y + 1$ as a functor. We refer to $y$ as a *functorial variable*. One can think of a polynomial simply as a data structure for an arena.

---

[Polynomial Functors: A General Theory of Interaction](https://topos.site/poly-book.pdf)
* Book by Spivak and Niu building on the below ref

[Poly: An abundant categorical setting for mode-dependent dynamics](https://arxiv.org/abs/2005.01894) (2020)
* Introduction to category $Poly$
