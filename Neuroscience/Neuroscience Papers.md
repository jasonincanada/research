[Right frontal anxiolytic-sensitive EEG ‘theta’ rhythm in the stop-signal task is a theory-based anxiety disorder biomarker](https://www.nature.com/articles/s41598-021-99374-x) (2021)
* First theoretically-based biomarker for anxiety - goal-conflict-specific rhythmicity


[Hippocampal Spatial Mapping As Fast Graph Learning](https://arxiv.org/abs/2107.00567) (2021)
* Figure 3 strongly reminiscent of the idea behind `gridpass.io`
* Solo paper from a thinktank
* Emailed author in July 2021 #contact

[Rotational Dynamics Reduce Interference Between Sensory and Memory Representations](https://www.nature.com/articles/s41593-021-00821-9) (2021)
* Interesting paper showing #rotation in neural representation of past sensory data to deconflict from new data

[Visual and linguistic semantic representations are aligned at the border of human visual cortex](https://doi.org/10.1038/s41593-021-00921-6) (2021)
* Visual and linguistic representations are *aligned in the brain*
* "Remarkably, the pattern of semantic selectivity in these two distinct networks corresponded along the boundary of visual cortex: for visual categories represented posterior to the boundary, **the same categories were represented linguistically on the anterior side**. These results suggest that these two networks are smoothly joined to form one contiguous map." (Abstract)

[A data-driven framework for mapping domains of human neurobiology](https://doi.org/10.1038/s41593-021-00948-9) (2021)
* "... neuroimaging studies have often served to reinforce the differences between concepts that originated in psychology, rather than to define new concepts grounded in brain function."

* Machine learning applied to ~20,000 neuroimaging articles
	* full-text articles
	* accompanied by coordinate-based fMRI data
	* ~600,000 physical coordinates mapped one-to-many to 118 non-overlapping brain structures
	* ~1,600 mental functions compiled from public sources (eg: "emotional memory", "retrieval", "face identification task")

* "To map links between the 1,683 terms for mental functions and 118 brain structures in our neuroanatomical atlas, we computed their co-occurrences across the training set. ... Circuits supporting distinctive sets of mental functions were then defined through $k$-means clustering of the brain structures ... over a range of $k$ values from 2 to 50."
* Paper concentrates mostly on $k = 6$
* Extended data fig. 2 shows $k = 2$, then $k = 3$, etc, gradually more detailed sub-clustering of functional domains.  Normal fig. 2 shows $k = 6$, $8$, and $22$, a fascinating rendering. Note the convergence of Recall and Retrieval domains from both Vision and Memory domains moving from $k = 8$ to $k = 22$
* "As $k$ increases across the hierarchy, domains at lower $k$ fractionate into subcircuits with more finely specified mental functions. For instance, **memory begins at $k = 6$** as a medial temporal circuit with affective and memory components, then is **subdivided at $k = 8$ into a memory domain with a hippocampal circuit and an emotion domain with an amygdalar circuit**. The $k = 8$ memory domain is then parcellated at $k = 22$ into domains for recall and encoding processes, and for semantic and episodic forms."
* Fig. 4 maps the new hierarchy at $k = 6$ to two leading expert-driven frameworks, RDoC and DSM
* "Neural circuitry need not align with human intuition for the structure of mental phenomena, and indeed the brain-based mapping of mental functions we present here yields several results that are unexpected from the psychology literature."
	* Before neuroimaging, psychology maintained a "circumplex model for emotion as a distinct processing domain with underlying axes for valence and arousal. ... However, in the data-driven arrangement at the $k = 6$ level, affective processes are integrated into circuits for memory and reward, consistent with the theory of constructed emotion proposed more recently to account for neuroimaging findings.
	* "Likewise, the data-driven framework combines stimulus and response processing stages, which have long been dissociated in psychology, under a single manipulation domain.
	* "Perhaps most surprising, the cognition domain spans a combination of terms for cognitive control, salience and emotion which is unrecognizable among the [RDoC](https://www.nimh.nih.gov/research/research-funded-by-nimh/rdoc/about-rdoc) domains."


[Neuronal sequences during theta rely on behavior-dependent spatial maps](https://doi.org/10.7554/eLife.70296) #Par21 (2021)

- Mathematically models an animal's positional representation within hippocampal theta oscillations via a new formula that matches the experimental evidence where the two existing (and conflicting) methods fall short

- "The first cells to fire typically have place fields centered behind the current position of the animal, followed by cells with place fields centered progressively ahead, generating so-called ‘theta sequences’" p. 1

- "This phenomenon suggests that beyond the representation of the current spatial location of an animal, the hippocampal theta code more generally encompasses representations of past, present, and future events" p. 1

- "... for the hippocampal theta phase code to be useful, there must be a consistent relationship between theta phase, represented position $r(t)$, and the animal’s true location $x(t)$. Surprisingly, this relationship has not previously been made explicit." p. 2


### two existing models (spatial/temporal)

In all three models below, $x(t)$ represents the actual position of the animal at time $t$, $r(t)$ the position represented by the hippocampus at time $t$, equal whenever the represented and actual positions are the same but at all other times different. Theta oscillation rates are ~8Hz so about eight times a second the hippocampal code sweeps from behind the animal in time/space, through it and onwards in time/space.  Existing lit falls within two models:

- *Spatial sweeps* (one theta cycle sweeps from a **position** starting behind the animal and ending at a position ahead of it):

$$r(t) = x(t) + d_\theta \frac{\theta(t) - \theta_0}{360}$$

- *Temporal sweeps* (one theta cycle sweeps from where the animal was a certain **time** ago, to where it'll be a certain time in the future):

$$r(t) = x\left(t + \tau_\theta \frac{\theta(t) - \theta_0}{360}\right)$$

- $\theta_0$ represents where in the theta cycle the represented and actual position are the same

- "Notably, the temporal sweep predicts different distances depending on speed of movement" p. 2

### proposed model (behaviour-dependent)

- "This third option combines the spatial sweep’s constant place field sizes and phase precession slopes with the temporal sweep’s increase in theta trajectory length with running speed. The former property requires that sweeps are independent of running speed whereas the latter requires that they depend on it. While at first this appears to be a plain contradiction, a resolution is offered if sweeps are made independent of the animal’s instantaneous running speed $v(t)$, but dependent on their ‘characteristic running speed’ at each position $\overline{v}(x(t))$." p. 4

$$r(t) = x(t) + \overline{v}(x(t))\tau_\theta \frac{\theta(t) - \theta_0}{360}$$

- The characteristic speed is the instantaneous speed the animal typically attains at a given position.  Equivalent to the spatial sweep model with theta distance (full extent of sweep) dependant on the characteristic speed at every position:

$$d_\theta = \overline{v}(x(t))\tau_0$$

### comparison

- "The temporal sweep model roughly captures the observed increase in theta trajectory lengths, place field sizes and phase precession slopes combined across different positions and fields based on instantaneous running speed. However, it did so for the wrong reasons, since it incorrectly predicts changes in individual fields with speed (Figure 7B)." p. 13

- "By contrast, the spatial sweep model accounts for the speed-independence of individual fields, but severely undershoots the increase in theta trajectory length with running speed and fails to capture the increases in place field sizes and phase precession slopes (Figure 7C)."

- "Only the behavior-dependent sweep model is able to replicate the correct combination of qualitative effects (Figure 7D). Furthermore, the behavior-dependent sweep produced values with the lowest mean squared deviation to the experimental data for four of the five variables considered (Figure 7; numbers in corners)."

Figure 7: ![[par21 fig 7 - behaviour dependent sweeps.png]]

