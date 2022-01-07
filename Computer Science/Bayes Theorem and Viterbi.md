### Hidden Markov Models

[A friendly introduction to Bayes Theorem and Hidden Markov Models](https://youtu.be/kqSzLo9fenk)
[Viterbi Algorithm segment](https://youtu.be/kqSzLo9fenk?t=1349)

![[hidden markov model.png]]

Transition probabilities
![[hmm - transition probs.png]]

Emission probabilities
![[hmm - emission probs.png]]


### Bayes Theorem

Sunny or rainy, independent of Bob's mood:
![[bayes - priors.png]]

Posterior probabilities of the weather given that Bob is happy:
![[bayes - posterior.png]]

Probabilities of weather transitions given Bob's mood:
![[bayes - total probability.png]]

Maximum likelihood, model that makes the observations the most likely to happen:
![[bayes - maximum likelihood.png]]


## Viterbi Algorithm

[The Viterbi Algorithm : Natural Language Processing](https://www.youtube.com/watch?v=IqXdjdOgXPM)

Heart of the Viterbi algorithm is being able to discontinue paths that aren't maximum "from here on out"; e.g. in the following, beyond the 3rd column's NN there's no point continuing with the .00048 path
![[viterbi - pos tagging.png]]
