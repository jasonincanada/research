[Optimal routing to cerebellum-like structures](https://doi.org/10.1038/s41593-023-01403-7) #mus23 (2023)

"... More generally, it shows that structured compression followed by random expansion is an efficient architecture for flexible computation." (Abstract)

- cerebral cortex processes input with highly connected recurring networks
- by contrast cerebellum-like structures are largely feed-forward to a sparse granule cell (GrC) layer that lacks recurrence
- prior theories assumed independent inputs, but this underestimates learning capability
- "bottleneck" architecture pre-synaptic to GrC theorized to facilitate downstream learning despite input correlations and task-irrelevant activity

"We show that the functional role of these pre-expansion bottlenecks is best understood in conjunction with the computations performed by the downstream GrC layer." p. 2

![[mus23 fig 1abc - schema.png]]
**Figure 1** **a)** insect olfactory system **b)** cortex->pontine nucleus->cerebellum pathway **c)** diagrams showing common three-layer structure of compression followed by expansion. insect olfactory compression layer is smaller and contains recurrent connections (looping orange arrow)

## Model

Pathways to cerebellum-like structures are characterized by initial compression (reducing number of neurons) followed by expansion. Researchers model $N$ input layer neurons to $M$ granular cell neurons through a compression layer of $N_c$ neurons

- compression layer neurons have higher firing rates, represented with linear or rectified linear neurons
- expansion layer neurons are more sparse, represented as binary neurons

Activity of compression layer neurons on the input layer $\mathbf{x}$:
$$\mathbf{c} = G^{FF}\mathbf{x}$$

Add recurrent connections if needed with a matrix $G^{rec}$:
$$\mathbf{c} = (I - G^{rec})^{-1}G^{FF}\mathbf{x}$$

Expansion layer:
$$\mathbf{m} = \Theta(J\mathbf{c} - \theta)$$

- $G^{FF}$ is a matrix of feed-forward connections from input to compression layer
- $\mathbf{x}$ are the input layer neuron firing rates as an $N$-dimensional vector
- $J$ are connections from compression to expansion layer
- $\Theta$ is the [Heaviside step function](https://en.wikipedia.org/wiki/Heaviside_step_function)
- $\theta$ are the firing thresholds of expansion layer neurons

"In our model, the network learns a mapping from patterns in a D-dimensional task subspace of the input layer activity to the target activation of a readout of the expansion layer, with D ≪ N. This contrasts with previous work that has typically assumed high-dimensional, random and uncorrelated input patterns." p. 2

- task subspace holds the inputs relevant to the current task

"We consider two classes of input representations, corresponding to different organizations of selectivities of input neurons to the task variables. In a clustered representation, input neurons belong to distinct groups, each of which is selective to a specific task variable. ... In contrast, in a distributed representation, each neuron is tuned to different linear combinations of multiple task variables. Our central contribution is a theory that relates these two classes of input representation to predictions about the compression architecture that optimizes downstream learning by the expansion layer." p. 3

![[mus23 fig 1d - two repr classes.png]]
**Figure 1d** "Example of clustered and distributed input representations. A smooth trajectory z in a two-dimensional task space (center) is embedded in an input representation of six neurons."

## Results sections

**Selectivity to task-relevant dimensions determines learning performance**
**Optimal compression for clustered and distributed representations**
**Compression of clustered representations in the insect olfactory system**
**Compression of distributed representations in the corticocerebellar pathway**
**Optimal in-degree of learned corticopontine compression**
**Feedback from the deep cerebellar nuclei improves selection of task-relevant dimensions**
**Hebbian compression can explain correlation and selectivity of GrC**
**Bottleneck architecture is more efficient than a single-step expansion**

"In total, we find that recurrence is necessary to decorrelate clustered input representations, while it is dispensable for distributed input representations as long as input redundancy is sufficiently high." p. 4

"The anatomy of the corticocerebellar system suggests a solution to this problem: in addition to cortical input, the pontine nuclei also receive feedback from the deep cerebellar nuclei (DCN)—the output structure of the cerebellum. Previous theories have largely ignored these connections. We provide a new interpretation of this motif and suggest that it provides a supervisory signal that aids the identification of task-relevant inputs." p. 7

"In summary, our results support a new functional role for DCN projections to pontine neurons: enabling the extraction of task-relevant, but subleading, input components." p. 7

## Discussion

"Our results demonstrate that specialized processing in ‘bottleneck’ structures presynaptic to granule-like expansion layers substantially improves the quality of expanded representations. This two-step architecture, with a structured bottleneck followed by a disordered expansion, is also more efficient, in terms of total number of synapses, than a single-step expansion. The circuitry that optimizes performance depends on input statistics, with clustered and distributed input representations leading to different predictions about compression architecture." p. 9

## Methods

Recurrent interactions in compression layer can be modeled with a differential equation:
$$\tau_c \dot{\mathbf{c}} = -\mathbf{c} + G^{rec} \mathbf{c} + G^{FF}x$$

Authors assume $\tau_c$ is much smaller than the input-varying timescale to focus on steady-state dynamics (p. 13):
$$\mathbf{c} = G^{rec}\mathbf{c} + G^{FF}\mathbf{x} \implies (I - G^{rec})^{-1}G^{FF}\mathbf{x} =: G^{eff}\mathbf{x} $$
