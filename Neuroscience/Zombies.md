[Neural mechanisms of parasite-induced summiting behavior in ‘zombie’ _Drosophila_](https://doi.org/10.7554/eLife.85410) #ely23 (2023)

See [[Fruit Fly]]

Summit disease:
- frequently seen behavior manipulation in parasitized insects
- "... induced by diverse parasites, ranging from viruses to fungi to trematodes, and affects a broad range of insect species, including ants, beetles, crickets, caterpillars, and flies."
- "The most consistently reported symptom of summit disease is elevation prior to death. This positioning advantages the parasite by either making the spent host more conspicuous, and therefore, likely to be consumed by the next host in its life cycle ..., or by positioning the spent host for optimal dispersal of infectious propagules." p. 2

Other examples of parasitism:
- ‘zombie ant’ fungus *Ophiocordyceps unilateralis* compels host ants to leave their nest, wander away from foraging trails, scale nearby stems, clamp onto vegetation, die, then rain down spores on the ground below. YouTube video from Real Science (not mentioned in study): https://www.youtube.com/watch?v=jM5jf-8ekVA&t=86s
- jewel wasps subdue cockroaches
- protozoans suppress rodents' fear of cat odors
- worms drive crickets to leap to watery deaths

### *Entomophthora muscae* 

Study focuses on fungal parasite *Entomophthora muscae*:

- infection begins when spore lands on fruit fly's cuticle
- enters hemolymph and begins to replicate, first using fat body (liver-like store of nutrients) of the host until the fat body is exhausted
- then starts the same three typical behaviors to get the fly into position for the next cycle:
    - summiting
    - extending its proboscis, which glues the fly in place
    - fly’s wings lift up and away from dorsal abdomen, making way for spores to disperse
- "Fungal structures ... then emerge through the cuticle and forcefully eject infectious spores into the surrounding environment via a ballistic water cannon mechanism." p. 2

### Time of day

Time of day is a big feature of fungus-induced summiting:

- *E. muscae* (study's focus) kills fruit flies around sunset
- *Ophiocordyceps* kills host ants around solar noon
- *Entomophaga grylli* kills grasshoppers within 4 hours prior to sunset
- *Erynia neoaphidis* kills aphids around 8.5 hours after sunrise
- *Entomophthora planchoniana* kills aphids around 14 hours after sunrise

![[ely23 fig 1e - time of death - e muscae.png]]
**Figure 1E:** Distribution of time of death for flies infected with *E. muscae*

This shows infected fly deaths concentrated in the final hours of the day. Compare this to uninfected flies that die from starvation:

![[ely23 fig 1s2c - time of death - starvation.png]]
**Figure 1S2C:** Distribution for uninfected flies

"As expected, wild-type flies killed by *E. muscae* tended to die in the evening, but there was variability in the timing of death. ... *E. muscae*-exposed flies continued to die at specific times of the day even in complete darkness, suggesting that the timing of death is under circadian control. " p. 3

![[ely23 fig 1s1b - circadian timing.png]]
**Figure 1S1B** Infected flies still die at the same time in darkness

## Y position and burst of locomotion 

Key signs of *E. muscae*-induced summiting are higher final y position of host and a burst of locomotion before death:

![[ely23 fig 1f - speed and y pos.png]]
**Figure 1F**: Relative y position in arena and average locomotion speed in the 12 hours before death from infection. The arena is basically a transparent straw with one hole plugged with food, the other with cotton

Compare this to the speed of uninfected flies in the 12 hours before death from starvation:

![[ely23 fig 1s2a - speed starvation.png]]

"These experiments suggest that an increase in speed ~2.5 hr before death and dying at specific times are signatures of *E. muscae* mortality." p. 5

### Summiting behavior requires host circadian and neurosecretory pathways

"To determine what higher-level systems might be *E. muscae*’s target, we looked for enrichment of large effect sizes in the genes (or circuit elements) involved in the same higher-level functions (or brain regions). ... We found that neurons in the antennal mechanosensory and motor center (AMMC), subesophageal ganglion (SOG), circadian system, and pars intercerebralis (PI) were overrepresented in the quintile of most negative effect size. ... we observed that many of the neurons of large effect in the AMMC, SOG, and circadian system also innervated the PI. ... we saw a clear enrichment for genes expressed in circadian cells. Thus, our screen pointed conspicuously toward roles for the PI and the circadian network in summiting behavior." p. 6

"We noticed that several of our hits affected a subtype of clock neurons, the group 1 posterior dorsal neurons (DN1ps). DN1ps are a heterogeneous population of neurons numbering approximately 15 cells per brain hemisphere. ... Taken together, these results implicate DN1ps as mediating fungal manipulation while also revealing fine-scale complexity, as activity in some DN1ps, but not others, is required for full summiting." p. 8

"... This suggests that the main population of clock neurons upstream of DN1ps is irrelevant for summiting." p. 9

"We next tested whether the ectopic activation of DN1ps or R19G10 neurons could drive ‘summiting’ in flies that had never been exposed to *E. muscae*. ... ectopically activating DN1Ps and R19G10 neurons appear to robustly induce a summiting-like increase in activity in flies unexposed to the fungus." p. 10

### The corpora allata are post-synaptic to R19G10 (PI-CA) neurons and necessary for summiting

"In insects, pars intercerebralis neurons often project to the neurohemal organs of the retrocerebral complex (RC). We suspected this might be the case for R19G10 neurons. The RC in *Drosophila* consists of two pairs of fused neurohemal organs:" p. 10

- corpora cardiaca (CC), sole site of adipokinetic hormone (Akh) synthesis
- corpora allata (CA), sole site of juvenile hormone (JH) synthesis

"Overall, these results indicate that CA function is necessary for summiting, ..." p. 11

### A real-time, automated classifier for summiting behavior

The researchers developed a real-time video monitoring system to watch all 128 flies (each in its own arena) at the same time. The idea was to have an algorithm (a random-forest classifier) identify when a fly started summiting, so they could study the fungal infection in real time. Prior to the experiment, they trained the classifier on a dataset of ~20-hour recordings of speed/y-position from 1306 *E. muscae*-exposed flies, 345 of which were "zombies" (their term for infected flies that succumbed to the infection, compared to "survivors", which were infected but didn't die from it). p. 11

![[ely23 fig 4g - classifier.png]]

**Figure 4G:** Behaviour (top 2 panels) and class probability (bottom panel) showing the moment the fly was classified as summiting

"Finally, we configured our fly-tracking software to run the classifier concurrently and email the experimenter when a summiting fly was flagged. Thus, we had a convenient, high-accuracy tool for experiments requiring real-time identification of summiting flies." p. 13

### During summiting, *E. muscae* cells are adjacent to the PI and the PI-CA pathway appears intact

"Using the real-time classifier, we assessed the distribution of *E. muscae* cells within the brains of summiting flies. ... We observed a consistent pattern of *E. muscae* occupancy in the brain, with a plurality of fungal cells (27–41%) in the superior medial protocerebrum (SMP), the region that contains the PI. Notably, there were very few fungal cells in the central complex, a premotor region." p. 13

"Fungal cells appear to displace host brain tissue, sitting in ‘holes’ visible in actin-binding phalloidin counterstains. Consistently, the distribution of holes across brain regions was indistinguishable from the distribution of fungal nuclei. Occasionally, we observed holes within the axon bundle of PI-CA neurons, but there was no indication of broken axons. Our interpretation is that during summiting, fungal cells displace neuropil without substantially consuming neural tissue or severing neural connections. This is consistent with the logic of zombie manipulation: *E. muscae* only consumes host tissues once they have served their purpose in aiding fungal dispersal." p. 13

"While the brain is largely intact in summiting, this is not the case for organs in the abdomen, which are essentially obliterated in summiting flies. The state of the abdominal organs is striking considering that these flies walk apparently normally." p. 13

![[ely23 fig 5g - organs of host.png]]

**Figure 5G:** The obliterated organs of a summiting vs non-summiting infected host. "Left: Infected, non-summiting fly (96 hr after exposure to fungus). Right: summiting, _E. muscae_-infected fly. a=abdomen, b=brain, w=wing, m=muscle. Scale bars are 200 microns. Insets of the abdomen and brain are shown for each fly below (scale bars are 25 microns). Host tissues are outlined in dashed black; black arrowheads indicate fungal nuclei."

"We observed extensive degradation of host abdominal tissues in summiting animals. We were stunned to find flies with obliterated guts and gonads walking apparently normally. Despite widespread destruction in the body, the CA and PI-CA neurons appear intact in summiting animals, which is consistent with an acute role in summiting." p. 21

"The CA resides in the thorax adjacent to the esophagus and proventriculus. We wondered if these tissues might be degraded like the abdominal organs in summiting flies. We used the classifier to collect summiting and non-summiting Aug21 >GFP animals and found that the CA was consistently present in summiting flies (as well as controls). Overall, the preservation of the CA during summiting suggests that its function is needed to mediate summiting behavior." p. 13

### Evidence for the metabolic induction of summiting behavior

"We wondered if *E. muscae*’s invasion of the brain disrupts the fly’s blood-brain barrier (BBB). Like vertebrates, flies maintain a BBB that restricts the diffusion of compounds circulating in the hemolymph into nervous tissue. ... We found that BBB permeability was higher in exposed flies versus controls at 98 hr after exposure. ... Our data are consistent with BBB permeability-increasing with time since exposure." p. 13

"We next used LC-MS metabolomics to compare the molecular composition of hemolymph in summiting flies to that of exposed, non-summiting flies. ... Many of the compounds could not be identified. These included three compounds that were uniquely detected in summiting flies ($C_6H_8N_2O_3$, $C_{14}H_{16}N_6O_7$, and $C_{12}H_{19}N_2PS)$" p. 15

### A neuro-mechanistic framework for summiting behavior

"Altogether, our experiments point to a series of mechanisms by which *E. muscae* induces zombie summiting behavior. The fungus invades the brain as early as 48 hr prior to death, establishing extensive SMP occupancy by at least 24 hr before death. When summiting behavior begins ~2.5 hr prior to death, the fungus has altered host hemolymph, likely via secretion of secondary metabolites. We hypothesize that these metabolites lead to the activation of PI-CA neurons, potentially via upstream DN1p clock neurons. In turn, we suspect that PI-CA activation stimulates the CA, leading to the release of JH. This hormone ultimately feeds back on the nervous system to generate the increase in locomotion at the heart of summiting. This framework unites the observations from many experiments and provides several specific hypotheses that we aim to tackle in future work." p. 17

![[ely23 fig 7 - sequence.png]]

**Figure 7**: Proposed sequence of summiting mechanisms in zombie fruit flies infected with *E. muscae*

## Discussion

"The evolutionary logic of targeting the circadian network is elegant: strains of *E. muscae* have been reported to infect and manipulate a diverse collection of dipteran hosts. The proximate motor circuits controlling locomotor activity may vary from species to species, but all flies have a clock and the clock exerts a strong influence on locomotor behavior. Targeting the clock network and downstream neurosecretory neurons may represent a simple, conserved mechanism to appropriately activate motor programs across host species." p. 19

### Morphological correlates of summiting

"Previous analyses of infection progression suggested that the fungus was not occupying the brain with any spatial specificity, but here we found otherwise. There is a clear pattern of fungal cells densely invading the SMP of summiting flies, a neuropil that harbors DN1p axons and PI-CA cell bodies and dendrites." p. 20

### Physiological correlates of summiting

"Cytosine is a pyrimidine nucleobase used in both DNA and RNA, a core molecular building block. It is intriguing that it was only detected in fungus-exposed fly hemolymph." p. 21

### A mechanistic framework for summiting behavior and beyond

"Our experiments have revealed key mechanisms likely to underlie the summiting behavior of zombie flies. *E. muscae* cells perturb the activity of circadian and neurosecretory neurons, leading to the release of JH and a resultant increase in locomotion. This effect is at least partially mediated by summiting-specific factors circulating in the hemolymph. Of course, many questions remain:
    - What compounds mediate the effect of transfused hemolymph?
    - What cells are targeted by these compounds and by what molecular mechanisms?
    - Do the fungal cells need physical access to the brain to induce a full summiting response?
    - Is the proximity of fungal cells adjacent to DN1p axons and PI during summiting merely a coincidence?" p. 22

"The dispersal and survival of *E. muscae* depend on a robust summiting response in the host, and the co-evolutionary relationship between these species likely extends back 200–400 million years. Such a robust strategy is unlikely to rely on a single perturbation that could be countered by simple evolutionary changes in the host. An increase in locomotion can be achieved in many ways and is the likely output of many different behavioral circuits, so it would be unsurprising to find that multiple host circuits are targeted, including others yet to be discovered." p. 22
