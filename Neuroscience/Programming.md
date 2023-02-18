[Programming experience associated with neural efficiency during figural reasoning](https://doi.org/10.1038/s41598-020-70360-z) #hel20 (2020)

- study tested programmers vs. non-programmers on three types of reasoning tests:
    - **FIR** - figural inductive reasoning
    - **NIR** - numerical inductive reasoning
    - **VDR** - verbal deductive reasoning
- EEG measured changes in alpha and theta power

### Prior studies

- FIR particularly relevant to programming
- increase in cognitive load associated with changes in two EEG frequency bands
    - decrease in alpha (8–12 Hz) power (event-related desynchronization, ERD)
    - increase in theta (4–8 Hz) power (event-related synchronization, ERS) p. 2
- dual-process theory:
    - mental activity in reasoning and decision making is categorized by two types of processing:
        - type I: more automatic and capacity-free processes
            - fast
            - high capacity
            - independent of working memory
            - relatively light frontal executive functioning
        - type II: more controlled and capacity-limited processes
            - slow
            - low capacity
            - heavily dependent on working memory
            - linked to frontal executive functions (top-down control)
            - "reflect the activity of a supervisory attention system, specialized in monitoring and regulating the activity in other cognitive/neural systems"
        - both types highly interdependent

In this study "we hypothesize that programmers, who should show a superior performance especially in figural reasoning, display more efficient neural processing probably due to a more effortless and automatic task processing (type I processes) as compared to non-programmers." p. 2

### Experimental setup

- 41 university students, 20 with programming experience, 21 without
- 21 tasks per type (FIR, NIR, VDR), each task being of one of low / medium / high difficulty (7 each)
- all items presented in the same order to each participant
- 30 minutes per task type to complete all 21 items
- after each sub-test, participants could offer free-form explanations of their strategies, as many as they wanted
- data from only correctly-answered items were analysed

### EEG

- EEG measured with 60 electrodes
    - baseline measured first
    - decreases in EEG power while thinking, compared to baseline, result in negative values (event-related desynchronization - ERD)
    - increases in power result in positive values (event-related synchronization - ERS)
- alpha band (8–12 Hz)
    - ERD (decrease) of alpha "is associated with neural activation since alpha oscillations are related to an inactive resting state as well as active inhibition of brain areas where alpha oscillations are pronounced strongly." p. 5
    - predominant in healthy humans in posterior brain regions
    - alpha ERD seen while performing perceptual/judgment/memory/motor tasks
- theta band (4–8 Hz)
    - ERS (increase) in theta associated with encoding new information, episodic/working memories
    - mainly seen in frontal midline area

### Test types

- Figural Inductive Reasoning - **FIR**
    - have to infer rules governing 3x3 matrices of figures
    - bottom right field is empty and has to be inferred
    - there's a "none of the above" option to prevent response elimination (same for other two sub-tasks)
- Numeric Inductive Reasoning - **NIR**
    - 7 numbers in a row
    - have to infer rules governing their generation and generate the 8th one
- Verbal Deductive Reasoning - **VDR**
    - syllogism tasks
    - two statements (premises, assumed to be true) followed by four possible conclusions to draw from them 

#### Sample test items

![[hel20 fig 1 - sample items.png]]

### Results

- only in FIR, analysis showed a significant main effect for programmers vs. non-programmers
- across all three test types, programmers performed better in medium- and high-complexity tasks, but not low-complexity
- all participants did progressively worse as problems increased in complexity. p. 7
- no effect for gender, age

#### Mental strategies

- no large difference in mental strategies between programmers/non
- for strategy "*Finding differences in response options*" only programmers reported using it, and only for FIR
- for strategy "*Rejecting wrong answers step by step*" only programmers reported using it for NIR (both groups used it for FIR/VDR)
- only for FIR tasks, both groups used strategies focusing on the elements (number/position/shape/rotation), and analyzing them by their row/column
- only for NIR tasks were neighbouring items analysed
- only for VDR tasks were abstract thinking, deductive reasoning, and visual imagery used

**Table 2** - Relative frequencies of reported mental strategies (all blank cells are 0.00 values that I erased from the screenshot to leave only non-zero values):
![[hel20 table 2 - mental strategies.png]]

Participants could report more than one strategy per task.

#### EEG power changes

- both groups showed more pronounced alpha power reduction as complexity increased
- only programmers showed lower ERD for low-complexity tasks vs medium/high
- for NIR tasks, non-programmers showed higher ERD in the left hemisphere
- no effect for VDR tasks

**Figure 2** Alpha power changes
![[hel20 fig 2 - alpha topography.png]]

### Discussion

"Programmers showed higher behavioral performance levels as well as a more efficient neural processing in the figural reasoning task compared to non-programmers. No differences in behavior or indices of neural efficiency were observed in the verbal or numerical reasoning tasks." p. 9

"While all three reasoning tests used in the present study require problem-solving abilities, which are highly interrelated with both programming and CT [computational thinking], FIR specifically requires figural, rather than numerical or verbal processing. ... Ambrosio et al. showed that the grades of college students at the end of their first programming course correlated with their spatial reasoning ability ... at the beginning of the course. Likewise, a meta-analysis on programming interventions ... discovered a positive influence of the interventions on spatial skills, which include spatial reasoning." p. 9

"Both FIR and NIR are tests on inductive reasoning and, thus, the difference between the two tests is that only NIR requires numerical processing, which is not assumed to be a part of CT. Therefore, the distinction between CT and numerical abilities might explain why programmers outperformed non-programmers in FIR, while performing equally well in NIR." p. 10

"Our results indicate that the ability of figural reasoning is closely related to programming experience and, thus, could be a fundamental component of CT skills, which are required for programming." p. 10

"Only programmers showed differences in brain activity between the three complexity levels of the FIR task. Programmers showed decreases in brain activity with decreases in task complexity. ... No such complexity-specific differences were found in non-programmers. Hence, the superior behavioral performance in the FIR task in programmers compared to non-programmers goes along with a more efficient allocation of neural processing. Programmers seem to need less neural resources to solve the easier FIR tasks while the non-programmers are already more strongly activated during the easy FIR tasks, although no differences between groups were present in behavioral measurements." p. 10

"A more efficient neural processing in programmers might be a sign that programmers showed a stronger involvement of automatic, capacity-free type I cognitive processes, especially in easy FIR tasks, while non-programmers activated more cognitive-demanding type II processes leading to a stronger brain activation. Hence, programmers might have been more likely to process simple patterns and did not need extensive logical reasoning to decide upon the correct answer in easy FIR tasks." p. 10

"Both groups showed an increase in alpha and theta coherence with increasing task complexity. Hence, a stronger functional fronto-parietal connectivity was observed in more difficult [compared to] less difficult figural reasoning tasks. This indicates that with increasing task complexity, frontal areas need to exert stronger supervisory control over parietal areas." p. 11

---

[Software Bug Detection Causes a Shift From Bottom-Up to Top-Down Effective Connectivity Involving the Insula Within the Error-Monitoring Network](https://doi.org/10.3389/fnhum.2022.788272) #cas22 (2022)

### Introduction

"...a recent functional MRI (fMRI) study suggested a pivotal role of the insula during error-monitoring when challenging deep-level analysis of code inspection was required. This raised the hypothesis that the insula is causally involved in deep error-monitoring." p. 1

"Healthy adult programmers participated in this 3T fMRI experiment. The activation maps evoked by error-related events confirmed significant activations in the insula. Importantly, a posterior-to-anterior causality shift was observed concerning the role of the insula: in the absence of error, causal directions were mainly bottom-up, whereas, in their presence, the strong causal top-down effects from frontal regions, in particular, the anterior cingulate cortex [ACC] was observed." p. 1

### Paradigm

Participants were experienced software developers in the C language. They were given four tasks in random order:
- baseline (stare at a cross)
- natural language reading
- a C code snippet with no bugs
- a C code snippet WITH a bug

"To be able to evaluate the true error-related decision moments, the participants were also instructed to select a line as soon as they suspected the presence of a bug (“suspicion/eureka moment”) and to confirm the bug in the button “Bug” when they were sure that there was a fault (“Bug detection”)" p. 2

Researchers recorded fMRI data during these tasks

### Results

"The activation maps for the contrast of the Code with bugs vs. Neutral code (code without bugs) revealed the set of areas responding to the activity of searching for a bug during source-code understanding. In particular, we found activation in the bilateral anterior insula which is a pivotal hub within the salience network, in error-monitoring tasks, in particular, during bug monitoring. This insula activation was even more evident at the “eureka” moment of suspicion when the subject detects a bug in the code (Figure 3)." p. 4

![[cas22 fig 3 - brain activation map.png]]

"Taken together, our results suggest that the insula is a pivotal hub concerning reconfiguration of the directionality of the interactions as it becomes the target for an anterior shift of causal influences from frontal error-monitoring and executive function regions when bug detection is required. This region is driven mostly by posterior regions for the natural text reading and controlled by ACC when a very complex task of searching for bugs is required, connecting with frontal regions related to decision-making and error-monitoring within the salience network." p. 4

### Discussion

"Evidence that the insular cortex also seems to be involved in performance monitoring ... and our Granger causality findings showing that error-monitoring-related activity triggers a shift of causal influences to frontal regions, in particular, ACC, make a strong basis toward the notion that the insula is a pivotal region during error-monitoring." p. 5
