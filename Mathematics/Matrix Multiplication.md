[Matrix Multiplication Using Only Addition](https://doi.org/10.48550/arXiv.2307.01415) #cus23 (2023) #preprint 

[Discovering faster matrix multiplication algorithms with reinforcement learning](https://doi.org/10.1038/s41586-022-05172-4) #faw22 (2022)

- using machine learning to discover matrix multiplication algorithms that are more efficient than human-devised algos

"AlphaTensor discovered algorithms that outperform the state-of-the-art complexity for many matrix sizes. Particularly relevant is the case of 4×4 matrices in a finite feld, where AlphaTensor’s algorithm improves on Strassen’s two-level algorithm for the first time, to our knowledge, since its discovery 50 years ago." (Abstract)

- AlphaTensor improved [Strassen's](https://en.wikipedia.org/wiki/Strassen_algorithm) 4x4 matrix multiplication from $7^2 = 49$ multiplication ops to $47$ (in modular arithmetic, $\mathbb{Z}_2$)

---

![[faw22 fig 3 - algo summary.png]]

**Figure 3** Summary of complexity of known-vs-AlphaTensor-discovered algos. Numbers in red highlight new records

"From a mathematical standpoint, the diverse algorithms discovered by AlphaTensor show that the space is richer than previously known. For example, while the only known rank-49 factorization decomposing $\mathcal{T}_4 = \mathcal{T}_2 \otimes \mathcal{T}_2$ before this paper conforms to the product structure ..., AlphaTensor finds more than **14,000** non-equivalent factorizations (with standard arithmetic) that depart from this scheme, and have different properties ..." p. 51

---

Below is the newly-discovered 47-mult algo for multiplying 4x4 matrices in modular arithmetic ($\mathbb{Z}_2$). The $h_i$ are the 47 multiplications, the rest are simple additions. This was discovered by an algo, and it looks like it. Could this be re-rendered in some kind of human-meaningful format?

![[faw22 ext fig 1 - 4x4 with 47.png]]
