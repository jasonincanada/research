[Gated recurrence enables simple and accurate sequence prediction in stochastic, changing, and structured environments](https://doi.org/10.7554/eLife.71801) #fou21 (2021)

## Introduction

Two specific challenges in making predictions in real-life environments
- presence of randomness and change
- structure of the environment involves complex relationships

Two common approaches:
- Bayesian ("to derive statistically optimal predictions for a given environment knowing its underlying generative model")
    - but: "a specific Bayes-optimal solution only applies to a specific generative model (or class of models). Bayesian inference therefore says little about the algorithms that the brain could use"
- heuristics
    - easy to compute and accurate in specific enviros
    - but lacks generality
    
Thus the following questions:
- "Is there a general, biologically feasible architecture that enables, in different environments, solutions that are simple, effective, and that reproduce the qualitative aspects of optimal prediction observed in organisms?"
- "If so, what are its essential mechanistic elements?"


## Results

- all agents simulated in silico with the same challenge: sequence prediction: 

![[fou21 fig 1a - sequence prediction.png]]

- focuses on recurrent neural networks
- all architectures use same 3-layer template:
    - one input unit to code for current observation
    - one output unit to code for predicted next observation
    - a number of recurrent units between the two

![[fou21 fig 1b - template.png]]

- three mechanisms of recurrent neural networks identified which give them certain computational properties:
    - **gating**, for multiplicative interactions between the activities of units
    - **lateral connectivity**, for the activities of different recurrent units to interact with each other
    - **training of recurrent connection weights**, for adjusting the dynamics of recurrent activities to the training environment

![[fou21 fig 1c - three mechanisms.png]]

- an architecture with all three of the above is called a *gated recurrent* architecture. removing one of the three mechanisms yields certain effects:
    - without **gating**, there are no multiplicative interactions between activities (reduces to plain recurrent neural network)
    - without **lateral connectivity**, recurrent units are independent of each other; each unit acts as temporal filter on the input
    - without **recurrent weight training**, recurrent activity dynamics are independent of the environment and only the output unit's parameters can be trained

![[fou21 fig 1d - network architectures.png]]

- all networks in article have 11 recurrent units unless otherwise stated
