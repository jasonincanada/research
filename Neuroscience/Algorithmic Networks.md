[Different computations over the same inputs produce selective behavior in algorithmic brain networks](https://doi.org/10.7554/eLife.73651) #jaw22 (2022)

"... despite considerable progress, we have yet to understand where, when, and how specific algorithmic computations in the pathways dynamically represent and transform the visual input into integrated features to produce behavior" p. 2

"We framed this broad problem using the classic logical functions XOR, AND, and OR, in which different algorithms are required to produce correct responses from the same input stimuli. XOR is famously a nonlinearly separable function, whereas AND or OR is linearly separable, implying nonlinear vs. linear transformations of the same inputs in the considered architectures. We aimed to reverse engineer the different stages of linear and nonlinear computations in brain networks that implement the algorithms." p. 2

"Each task shows a similar dynamic unfolding: the first two stages represent and linearly discriminate the visual inputs; the third and fourth stages nonlinearly integrate them in a task-specific manner, revealing the solution of each task in the responses of individual MEG sources." p. 3

![[jaw22 fig 1 - XOR task.png]]


### Four systems-level stages of computation link stimulus to behavior

"The network model of Figure 1A schematizes these stages. Specifically, we show:

1. **Linear, contralateral discrimination of each input state separately (‘Lin’) in V1-4 regions with onset from ~60ms poststimulus**, quantified as the product of and the LEFT/RIGHT representation pattern metric and the multivariate R2 of a linear model for each binary input, color coded in light blue for the left input, in orange for the right input.
2. **Linear discrimination of both inputs (‘LinBoth’) on the same occipital and ventral sources ~100ms poststimulus**, quantified as the product of the BOTH representation pattern metric and the multivariate R2 of a linear model considering both inputs with no interaction, color coded in magenta.
3. **Nonlinear integration of both inputs (‘NonLin’) for task performance (XOR, AND, or OR) in temporal-parietal regions ~260ms**, quantified as the product of the XOR representation pattern metric and the significant improvement in model fit with interaction term, color coded in green
4. **Nonlinear integration of both inputs together with response-related activity (‘NonLin&RT’) in postcentral gyrus ~400ms**, quantified as mutual information (MI) between the 2D MEG magnetic field and RT on the corresponding trial, also thresholded by the product of the XOR pattern metric and the model interaction term, color coded in yellow." p. 5

Detailed dynamic unfolding described on p. 6


## Video

Online video: [Dynamic summary of the four stages of computation in the XOR task](https://elifesciences.org/articles/73651/figures#fig1video1)
