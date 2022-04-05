[Hippocampal replay reflects specific past experiences rather than a plan for subsequent choice](https://doi.org/10.1016/j.neuron.2021.07.029) #gil21 (2021)

- Study resolves limitations and ambiguities in prior studies that try to discern role of hippocampal replay, between two main hypotheses, *planning* and *memory storage*
    - replay for *planning* studies exclude "spatially and temporally remote, unavailable, or specific non-preferred options"
    - replay for *memory storage* studies were based on simple tasks with repeated navigation to small number of fixed locations

"Our results revealed a striking lack of correspondence between replay content and upcoming choice. Replay neither increased nor decreased the tendency of the subject to visit the replayed location, regardless of reward history or visit recency of the location. Instead, we found that replay was dominated by two categories of past experiences: places that had a reliably delivered reward (even after they no longer did so) and places that had not recently been visited, **strongly suggesting that hippocampal replay supports memory processes** by facilitating memory maintenance and long-term storage rather than by guiding subsequent behavior." p. 3150

Study ignores direction of replay, ie: whether forward or reverse: "Given the complexity of this distinction, and because we were primarily interested in assessing the spatial locations represented across as many events as possible, we did not separate events by directionality." p. 3153

---

[The content of hippocampal "replay"](https://doi.org/10.1002/hipo.22824) #Pfe17 (2017)

(This one is difficult to synopsize since it seems almost every sentence is substantial--I could almost paste the whole article into these notes. The article itself is a synopsis of several research papers. For conciseness I have elided all inline references. All bold emphasis was added by me. Page numbers are as labeled on the published pages, not the PDF viewer offset)


### 1 | Introduction

- damage to the medial temporal lobe (hippocampus in particular) impairs the forming of new episodic and spatial memories
- during exploration, individual hippocampal neurons code for spatial information in their firing patterns
- hippocampus as a spatial map was first reported in a short 1971 [article in Brain Research](https://doi.org/10.1016/0006-8993(71)90358-1) by O’Keefe and Dostrovsky

- central question: how is the experience and storage of a trajectory represented in the hippocampus, usually across tens of thousands of neurons, and how is the right information retrieved exactly when needed?

- one theory: ripples and ripple-based replay

"Ripples are brief (50–100 ms duration), high-frequency (150–300 Hz) network oscillations within the hippocampus which emerge during non-exploratory states such as slow-wave sleep, quiet rest, grooming, and eating/drinking, and disruption in their expression results in significant memory impairments" p. 6

![[pfe17 fig 1a - hippocampal ripple.png]]
- Figure 1a:  A hippocampal ripple.  Simultaneous recording of 91 CA1 place cells from a rat walking along a 1.8m linear track. Right-side timeslice is expanded to show a compressed representation of the trajectory **playing in reverse** from the rat's current location, after the traversal has finished

"Intriguingly, the content of ripple-based activity patterns can range between **forwards-ordered or reverse-ordered replay of prior behaviors, prediction of future actions, or even assimilation of independent experiences into a novel creation**. Thus, terms commonly used to describe this phenomenon, such as “replay” or “reactivation,” fail to adequately capture the diversity of function which these events likely represent." p. 7


### 2 | Early studies indicate that sleep replay replicates prior neuronal activity patterns

"Interpretations of early results were heavily influenced by prominent theoretical models which described a two-stage process for memory formation. Briefly, the models proposed that initial experience produces a labile and likely transient memory trace in the hippocampal network via activity-dependent plastic changes to the circuit. During subsequent “off-line” states (e.g., sleep), repeated ripple-based reactivation of precise hippocampal neural sequences associated with prior behavior was hypothesized to either consolidate those plastic changes within the hippocampus or transfer the information to the slower-adapting cortical circuit for long-term storage." p. 8

These early models made sense for various reasons:

- "they provided an explanation for anterograde amnesia and temporally graded retrograde amnesia following hippocampal damage"
- "they brought together emerging discoveries in hippocampal plasticity and in vivo physiology to explain sequentially ordered memory"
- "they beautifully addressed the temporal credit assignment problem [see sec 3.3] by proposing that hippocampal reactivation would allow for the temporal compression of prior experience to bring action and outcome together within the same brief circuit-level activity pattern"

More on the two-stage model:

- neurons that are highly active during spatial exploration have higher overall activity during the next sleep
- pairs of neurons that fire within 100ms of each other during exploration tend to fire together during sleep after (and not before) the behaviour
- these post-experience pair-wise correlations are much stronger during ripples than at other times during sleep
- precise temporal order of firing during waking behaviour is preserved in sleep-based ripples
- sleep-based sequences are temporally compressed compared to the same sequences while awake


### 3 | Awake replay provides unexpected insights

- ripples occur not only in slow-wave sleep but during pauses in waking exploratory activity

"In a [groundbreaking study](http://doi.org/10.1038/nature04587), Foster and Wilson reported that awake replay did not always conform to the established pattern. Rather, awake reactivation, while still a temporal compression of prior activity, could progress **in the opposite temporal sequence** to that which had initially occurred during behavior, as if the prior neural activity patterns were being replayed in reverse"

- replicated by six other studies


#### 3.1 | Replay requires minimal experience

- experience-dependent synaptic plasticity is correlated with replay expression p. 8
- but reverse replay can arise after only a single traversal across a new environment
- "theta sequences": temporally compressed sequences of neuron activity, produced by spiking of neurons within theta oscillation phases during exploration
- theta sequences are poorly organized on the first lap in a new environment p. 9


#### 3.2 | Replay can encode temporally and spatially remote experiences

- awake reactivation events encode paths starting from the animal's current location and crossing the local environment
- replay can encode coherent trajectories in a physically separate and previously explored environment
- these spatially remote replays show that immediate sensory input doesn't exclusively determine replay content p. 9
- coherent replays occur up to 10 minutes after exploration, casting doubt on early synaptic trace model that suggested reverse replay arises from slowly decaying activity traces


#### 3.3 | Reward influences the content of replay

- replay might solve the "temporal credit assignment problem" (what is this? read [#Cic10](https://doi.org/10.1080/019697299125127) and [#Fos06](http://doi.org/10.1038/nature04587)) by combining representations of current outcome and prior behavior within a brief window of time p. 10
- representation of new versus familiar environments is elevated in replay
- rate of ripples significantly increased at rewarding sites in enviroment vs non-rewarding
- Ambrose et al. replicated the correlation between total ripple rate and reward level, but also found a significant correlation between number of reverse-ordered (but not forwards-ordered) replays and magnitude of the reward, suggesting
	- reverse replay may participate in memory consolidation of salient experiences
	- forward replay may serve as a memory retrieval system for planning future behaviors (see sec. 4)


#### 3.4 | Replay exhibits learned information

- is the information encoded in replay a direct copy of actual experience or something more complex? p. 10
- early studies were with simple tracks and stereotyped behaviours
- Davidson et al. among the first to use sufficient numbers of recorded neurons to look closer at information content of replay
- showed that virtual trajectories encoded in awake replay progress at constant velocities (~15-20x faster than animal's average)
- suggests ripples express learned info rather than actual experience
- a two-choice maze experiment lends support: "Despite the fact that the rats always traveled from the central arm to either the left or right arm during behavior, Gupta et al. observed replay events encoding a “shortcut” path from the left arm to the right arm, a path the rat had never actually taken, demonstrating mental assembly of distinct experiences into a coherent representation of the spatial relationships within the environment." p. 10
- similar effects revealed in study of unique combinations of forward- and reverse-replay at choice points in a three-arm maze


#### 3.5 | Related experiences can be combined in replay via ripple concatenation

- rats exploring a 10-meter-long track
- "Importantly, because the virtual velocity within replays was relatively constant, playback of a ten-meter trajectory required over half a second to complete, much longer than a typical 100 ms ripple. The authors observed while individual ripples themselves appear to be somewhat restricted in their temporal duration, replay of long spatial trajectories can be represented **by concatenating multiple ripples together**"

- how does a ripple in the middle of an extended replay “know” where the last ripple ended?  how are they coherently assembled?
- "A potential answer comes from a recent study in which hippocampal and entorhinal cortical activity was simultaneously monitored. During replay, the **medial entorhinal cortex (MEC), which communicates bi-directionally with the hippocampus**, can also display increases in ripple-band power"
- "Intriguingly, awake ripple-like events in MEC **temporally alternated with concatenated ripples in the hippocampus**, indicative of a recurrent loop of activity and further suggesting that the end representation of one hippocampal ripple within a longer chain may initiate a corresponding representation in the MEC, which can then send that information back to the hippocampus to allow the next concatenated ripple to start in that location"
- "...this process may underlie the fascinating feature of multi-ripple replay in which a single extended replay will intersperse both forwards- and reverse-ordered movement on consecutive ripples: the “re-ignition” of a chained ripple via MEC feedback may contain both location and momentum information, but the direction-specific population that is activated may be stochastically determined by the local hippocampal network rather than extra-hippocampal sources" p. 11

- inhibition of MEC:
	- reduces number of multi-ripple events without altering total ripple number
	- fragments spatial representations within replays


### 4 | Future representation in replay—"Replay" is not just replay

"A complicated picture of replay emerges in which ripples encode for sequences of learned information rather than simple replications of prior neuronal activity. In particular, an important functional distinction appears to exist between the information content of reverse-ordered replay and forwards-ordered replay.  By replicating prior activity patterns starting from the present and extending into the animal’s past, reverse replay seems ideally suited for memory consolidation of previous salient experience, linking result to prior action. In contrast, forward replay in the awake state seems more practically suited for utilizing previously formed memories to sample possible future outcomes. Indeed, several lines of evidence support this latter hypothesis" p. 11

- awake forward replay may serve to construct predictions regarding future actions
- "this form of memory expression tends to arise immediately prior to movement, suggestive of a planning or preparatory mechanism"
- replay can also construct novel shortcuts that have never been experienced before, suggestive of a role in imagining future possibilities


#### 4.1 | Forward replay can correlate with future behaviour

- in a two choice maze, following learning, forward replay content immediately prior to making the decision was significantly more likely to encode the correct than incorrect path
- similar findings in an open arena goal-navigation task
	- rats alternated between random foraging and goal-navigation
	- experimenters changed goal location daily and session was set up so that trajectories from start/finish were novel
	- while away from goal location, replay was strongly biased to encode trajectories from rat's current location to goal
	- indicates replay can rapidly assimilate prior knowledge with new information


#### 4.2 | Forward replay can encode paths to avoid

- in a 2017 study, rats were shocked at the end of a linear track
- during followup exploration, they consistently avoided the shock zone
- "Replays during these pauses reliably encoded trajectories leading into the shock zone immediately prior to the rat turning around, consistent with a model of replay as a memory retrieval system capable of providing outcome predictions. Importantly, though, in this study the replay denoted paths to avoid rather than paths to follow, indicating that the content of replay is used to inform rather than dictate future behavior, possibly by coordinating the reactivation of amygdala-based representations of the valence of the encoded experience." p. 11

"Instead, these data suggest that reverse replay may be primarily utilized in the initial formation of a mental map of a novel environment, serving to synaptically couple neurons that represent adjacent locations;"

"It is important to note, however, that reverse replay is reliably observed during exploration of highly familiar tracks, suggesting that it likely continues to serve additional purposes beyond initial memory formation."


#### 4.3 | Reverse replay does not facilitate goal learning in a familiar environment

"During open field navigation, replays that occurred after the rat arrived at the recently learned goal location did not display a bias to encode paths corresponding to its prior path, suggesting that reverse replay was not prominent in this task and may therefore be dispensable for the process of rapidly assigning novel salience to a familiar location." p. 12

"These data are at odds with a clear enhancement of reward-based reverse replay in linear tracks. While this may be partly explained by the fact that the open field environment was highly familiar in the open field study, the predictable reward location was novel every session, and it is reasonable to expect strong release of salience signals at that position. Instead, these data suggest that reverse replay may be primarily utilized in the initial formation of a mental map of a novel environment, serving to synaptically couple neurons that represent adjacent locations; once formed, other processes may flexibly assign value to specific positions within that cognitive map."

"A prediction from this hypothesis is that replay in a novel open arena should predominantly encode the rat’s prior behavioral path, even if the rat is performing a familiar, goal-directed task that was learned in a separate environment. It is important to note, however, that reverse replay is reliably observed during exploration of highly familiar tracks, suggesting that it likely continues to serve additional purposes beyond initial memory formation."


#### 4.4 | Forward replay correlates to behavior only prior to memory-driven action

"The encoding of paths leading to salient locations and the strong correlation between the content of replay and the rat’s future behavior was only observed prior to goal-seeking or active avoidance."

"In contrast, replays which occurred prior to simple exploration or random foraging were significantly less correlated to the animal’s future behavior in these studies."

"At first glance, these data seem to indicate that in the absence of a predictable, salient outcome, the content of replay was not effective at influencing behavior, suggesting the presence of a top-level “evaluator” that assesses the content and result of a forward replay and decides whether to utilize that information or not."

"However, Pfeiffer and Foster demonstrated that during goal-seeking periods, when the content of replay (rarely) encoded paths leading somewhere other than the goal location, the rat was still highly likely to follow these paths even though they often took the rat farther away from the learned goal, arguing against the evaluator model (or at least, arguing against a perfect, pure-reward-based evaluator)."


#### 4.6 | A simple model of goal-directed forward replay

- section proposes and rules out a naive breadth-first search algorithm for path planning (fig. 3)

"It remains unclear, however, how a particular path to a known goal is expressed out of the near infinite number of possible paths"


### 5 | Replay may reveal the underlying hippocampal circuitry

- ripples can be influenced by external inputs
- but these population-level events are largely dependent upon internal hippocampal circuitry
- Two high-profile studies by Dragoi and Tonegawa test whether sequential order of neurons during ripples may **correlate with subsequent behaviour** (?!)

[Preplay of future place cell sequences by hippocampal cellular assemblies](https://doi.org/10.1038/nature09633)
[Development of schemas revealed by prior experience and NMDA receptor knock-out](https://doi.org/10.7554/eLife.01326)

- hippocampus recorded before, during, and after exploration of a novel track
- "Surprisingly, neural activity during many pre-experience ripples appeared to be sequentially organized to reflect the order that the cells would eventually fire during subsequent exploration of the never-before-seen track, as if the hippocampus was “pre-playing” spatial paths that it would take in the future"
- subsequent work has explicitly tested the role of experience-dependent synaptic plasticity in replay expression and the authors reported no evidence of pre-play p. 15


###  6 | CONCLUSIONS

- "Reverse replay, biased strongly by novelty and reward, seems well-suited for modifying the circuitry of the hippocampus to consolidate learned spatial relationships, while forward replay appears capable of retrieving these stored representations to influence future behavior." p. 15
- how paths are selected remains unclear
- "no current evidence indicating that forward and reverse replays are generated via distinct network mechanisms"
- "Sleep and wake replay also seem fundamentally different, as blocking sleep-based replays impairs long-term memory without impacting place field representation, while preventing awake replays impacts working spatial memory and place field stability without globally impacting long-term memory"
