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
