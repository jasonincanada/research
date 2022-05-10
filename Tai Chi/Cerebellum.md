[Distinct representations of body and head motion are dynamically encoded by Purkinje cell populations in the macaque cerebellum](https://doi.org/10.7554/eLife.75018) #zob22 (2022)

### Introduction

"The cerebellum guides motor performance by computing differences between the expected versus actual consequences of movements and then adjusting the commands sent to the motor system." p. 2

- vestibular sensory organs are in the head
- prevailing view: reflex pathways transform balance/self-motion from head-centered to body-centered reference frame
- neck proprioceptors provide head position information for this transformation
- transform vitally relies on anterior region of cerebellar vermis:
    - PCs (Purkinje cells) project from region to fastigial nucleus, an area important for posture and balance
    - inhibition of region impairs pathways that detect changes of head position relative to body
    - studies of region in cats show individual neurons can encode both vestibular and neck information, providing a neural substrate for the transform

"However, these studies stopped short of establishing whether Purkinje cells integrate vestibular and neck proprioceptive signals to dynamically encode head or body movement.  Thus, a key question yet to be answered is: Does the cerebellum integrate vestibular and neck proprioceptive signals to provide a dynamic representation of body motion relative to space?" p. 2

- researchers recorded individual Purkinje cells in the anterior vermis of monkeys as they rotated them in the dark (to rule out visual interference) in three different ways
    - head only, body fixed (head-on-body)
    - body only, head fixed (body-under-head)
    - combined head and body

![[zob22 fig 1a - 3 purkinje cells.png]]

**Figure 1A** Readings from three individual Purkinje cells demonstrating their heterogeneity, during whole-body rotation (separate figures exist for head-on-body and body-under-head). Cell 1 shows both increased and decreased firing rates based on rotation direction (clockwise/counter-clockwise). The study doesn't point it out but it appears that firing rates drop close to 0 when the rotation velocity is around 90 deg/s in the non-preferred direction; in the excitatory direction the firing rate increase continues past 100 deg/s rotation and only seems to start leveling off after it; there the plot runs out, rotations past ~150 deg/s are not reported.  Cell 2 shows increased firing rates regardless of rotation direction. Cell 3 shows no appreciable change from baseline firing rate for one direction but an increase in rate for the other direction (study only rotated subjects about the vertical axis).  A total of $n = 73$ Purkinje cells were recorded, 32 called Type I (right-most pane above) and 41 Type II (left and middle cells above)

### Results

"We found considerable heterogeneity across individual Purkinje cells in their encoding of head versus body motion, with most (~75%) neurons dynamically encoding an intermediate representation of self-motion between head and body motion. These neurons, termed bimodal neurons, responded to both vestibular and neck proprioceptive stimulation and displayed head-position-dependent tuning in their sensitivity to vestibular stimulation. In contrast, a minority of cells, termed unimodal neurons, only responded to vestibular stimulation and unambiguously encoded the motion of the head in space.

"Across all cells, the linear combination of a given neuron’s response sensitivity to dynamic neck and vestibular stimulation alone well estimated its response during combined stimulation.

"Finally, we found that a simple linear combination model combining the responses of ~40 Purkinje cells could account for the more homogeneous responses of target neurons in the deep cerebellar nuclei (i.e., the rostral fastigial nucleus [rFN]) during applied self-motion.

"Our results provide the first evidence, at the level of single Purkinje cells, that a sequential transformation from a head-centered to body-centered reference frame occurs between the cerebellum and deep cerebellar nucleus to ensure postural and perceptual stability in everyday life." p. 3

**Most vestibular-sensitive Purkinje cells in the anterior vermis are also sensitive to stimulation of neck proprioceptors**

- The heterogeneity shown by different PCs in Figure 1A contrasts with the responses in areas in the anterior vermis *targeted* by the PCs. "Notably, vestibular-only neurons in the rFN and vestibular nucleus consistently show excitatory versus inhibitory responses for oppositely directed head movements." p.3 

**Linear combination of the Purkinje cells’ response can encode head and body motion**

- Individual PCs don't tell the whole picture, so researchers computed how many cells need to combine to generate patterns seen in downstream regions (rFN). "Importantly, ... we found that the weighted activities of ~40 neurons generated responses that well approximated those previously reported for bimodal rFN neurons (Figure 7C, red arrow) ... Thus, a population of 40 Purkinje cells could explain the dynamic representation of body motion across conditions, as well as robust encoding of vestibular stimuli as a function of static head position observed in bimodal rFN neurons." p. 12

![[zob22 fig 7c - purkinje ensemble.png]]

**Figure 7C** The red arrow shows that ~40 Purkinje cells together are required to generate responses similar to a downstream bimodal rFN neuron

The model so far assumed no input to the rFN neuron other than the PC projections, but the FN receives mossy fiber inputs from 3 other structures. Researchers added mossy fibers to the model in various ways and found "... the addition of such simulated mossy fiber inputs did not dramatically alter our estimate of the Purkinje cell population size required to generate rFN neurons responses (~50 versus 40)" p. 14
