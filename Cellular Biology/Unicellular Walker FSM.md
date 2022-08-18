[A unicellular walker controlled by a microtubule-based finite-state machine](https://doi.org/10.1016/j.cub.2022.07.034) #lar22 (2022)

Videos of cell walking:  [S1](https://www.cell.com/cms/10.1016/j.cub.2022.07.034/attachment/2aadf415-9323-48e0-9807-c392ca66aee0/mmc2), [S2](https://www.cell.com/cms/10.1016/j.cub.2022.07.034/attachment/684c4be1-4748-4585-80ef-0ac199fcd621/mmc3)

"The involvement of information processing in cell state transitions suggest that cellular behavior can be understood as an embodied computation." p. 1

"How can a single cell coordinate a walking gait without a nervous system?" p. 1

"We hypothesized that walking cells might be governed by finite-state automata with directed, processive movement arising from reproducible, stereotyped patterns of state transitions. ... Here, we ... show that *Euplotes eurystomus* walks with a cyclic stochastic gait displaying broken detailed balance and exhibiting elements of stereotypy and variability, in accord with a **finite-state automaton representation**." p. 2


### A reduced state space is sufficient to describe walking dynamics

![[lar22 fig 2bcd - 14-bit vectors.png]]

**Figure 2 bcd**: Cirral dynamics encoded as a 14-bit binary vector. **(d)** sample trajectory, white: cirrus up/moving; black: cirrus down/nonmoving

"Because our ultimate goal was to identify motifs among the patterns of cirral activity, which entail strictly non-negative values, we performed dimensionality reduction by non-negative matrix factorization (NMF), a technique used to identify patterns in a wide range of other contexts." p. 2

"NMF revealed the cirral states to be well-described by a 3D space." p. 2

![[lar22 fig 2efg - state space.png]]

**Figure 2 efg**: 3 orthogonal views of cirral gait state space after dimensionality reduction by NMF. Axes H1/H2/H3 are the NMF factors


### Euplotes walks with a cyclic stochastic gait

![[lar22 fig 3b - transition rates.png]]

**Figure 3b**: Gait state transitions showing broken detailed balance.  Eg. the rate from state 3 to 17 is higher than from 17 to 3

"Several analyses suggested that *Euplotes* retains some memory of the prior sequence of cirral movements during locomotion such that the gait may not conform to a continuous or discrete-time first-order Markov process. Taken together, our analysis revealed a mixture of unbalanced transitions driving cycles and balanced transitions arranged as networks, for which we propose to apply the term ‘‘cyclic stochastic gait.’’ It has been argued that physical systems exhibiting such a mix of stereotypy and variability can be viewed as performing computations in the sense that the evolution of the system over time is most compactly described as **the result of a computational process involving state transitions, memory, and decision rules.**" p. 6

"Altogether, the picture of stereotypical gait dynamics that emerges is one of biased transitions involving cycle states preceding relatively low-probability, unbiased transitions associated with substantial cell movement before returning to the start or cycle states and beginning the sequence again." p. 6


### The microtubule-based fiber system mediates gait coordination

![[lar22 fig 1c - drawing.png]]

**Figure 1c**: Drawing of a *Euplotes* cell, ventral surface, highlighting fiber system connecting cirri

"The complex yet sequentially structured gait patterns in conjunction with our simulation results are consistent with the existence of some form of nontrivial gait coordination. What physical machinery could embody the information processing required to generate the stochastic, cyclic state transitions seen during *Euplotes*’ walking?" p. 7

![[lar22 fib 4ab - fiber structure.png]]

**Figure 4ab**: Two distinct classes of fibers. Graph representation of fiber-fiber connections

"We reconstructed in 3D the microtubule-based fiber system of *Euplotes* ... we noted the presence of two morphologically distinct classes of fibers, one thicker and linear and the other thinner, splayed, and less linear ... Fibers emanate from the bases of all cirri, appear to intersect one another, and also intersect the cell cortex at various points." p. 7

"... these observations suggest a mechanism of mechanical coordination in which microtubule bundles allow groups of cirri to influence successive behavior of other groups of cirri." p. 7


## Discussion

"Traditionally, studies of computational processes in cells have focused on combinatorial logic, in which a molecular network generates an output that depends only on the current input. We have focused on sequential logic, in which outputs depend on the system state as well." p. 10

"We propose that in *Euplotes*, biased, actively controlled cyclic transitions store stress in certain cirri, and the spontaneous release of these cirri from the substrate, during a series of unbiased gait state transitions, allows the cell to move forward. Return to the cycle states reset this process by winding up the system for continued, proper cell movement." p. 10

"We conjecture that movement of cirri relative to one another can establish tension in the fiber system and that the tension state of fibers associated with each cirrus may then modulate cirral activity in a manner reminiscent of basal coupling in flagellates." p. 10

"Our results show that perturbation of the microtubule fiber system shift the gait of *Euplotes* from a regime of asynchronous yet coordinated movements to a dysregulated regime with synchronous yet improperly coordinated movements." p. 10
