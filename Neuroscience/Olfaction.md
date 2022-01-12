[Invariant odor recognition with ON–OFF neural ensembles](https://doi.org/10.1073/pnas.2023340118) #niz22 (2022)

Press release: [The ‘surprisingly simple’ arithmetic of smell](https://source.wustl.edu/2022/01/the-surprisingly-simple-arithmetic-of-smell/)

---

The sense of smell can reliably detect the same odor again even with environmental perturbations (overlapping odors, humidity, temperature, etc)

But neural responses to the odor at the single cell and ensemble level did vary with most of these perturbations.  So how is the overall odor detection made?


### results

"We found that there are two orthogonal ensembles of neurons, one activated during stimulus presence (ON neurons) and one activated after its termination (OFF neurons), and both contribute to this important computation in a complementary fashion." p. 1

- experimenters trained a linear support vector machine classifier (SVM)

"... a simple linear classification scheme was sufficient to extract the relevant information. The classifier essentially boiled down to **adding the contribution of PNs** that were strongly activated when the odorant was presented (ON neurons) and **subtracting the contribution of PNs** that were activated after the termination of the odorant (OFF neurons)." p. 8


### it gets simpler

Researchers found similar detection ability even when significantly simplifying the data set by mapping weights to the set $\{-1, 0, +1\}$ 

"We found that this simpler approach was still able to allow robust detection as well as discrimination of both the target odorants" p. 8


### but not too simple

"Further simplification of this approach by just using Boolean weights, $\{1,0\}$, allowed detection of the target odorant, but discrimination between the two target odorants was compromised"


### thoughts

This is reminiscent of the dominators from [[Dynamic Programming#Value decompositions and sets]] in #erw21, if we consider the OFF neurons from the current article as the **barrier**, and the ON neurons as **support**.  In this framing, with the above results, odor detection would be tantamount to support overcoming the barrier
