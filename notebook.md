This file serves as a kind of "lab book" documenting my working process.

### 09/02/24
Up until now, my progress consisted of trying to familiarize myself with some concepts from (Crutchfield & Feldmann 2001), implementing an approximation of the entropy of a fair coin flip with an increasing amount of data.
Today, an analysis on the MDP shown in "Affordance-based-PS-demo.ipynb" was done by looking at Markov processes (MPs) resulting from only observing the system.
One can create three different MPs, one only observing the state of the light, one only observing the rat's actions, and one observing both. When observing both, one has to choose how exactly the light state and action state are connected. I decided to look at combined states resulting from the current state of the light, and the action that was just performed to bring the system to that state.
One can then calculate the probabilities of each respective state of the mentioned MPs occurring, as shown in "first_steps.ipynb".

### 11/02/24
The graphs and calculations were now put into the jupyter notebook from handwritten notes, now also including the probability for the light turning on.

### 23/02/24
An attempt was made to calculate the transient information of a coin flip.
For this, two approaches were used, one calculating entropy etc. consistent with the explanations in (Crutchfield & Feldmann 2001), which looks at the entropy of sets of a given length.
The second approach looks at the estimation of the coin flip entropy by observing one coin L times and how this converges towards coin entropy.

### 27/02/24
Over the past few days the state probabilities for the three state MDP were approached.
In a book (C. Iben: Markov Processes for Stochastic Modeling), a method to find the limiting probabilities of a MP was described, using rather simple matrix calculations.
The results of this method are in perfect agreement with other results, for example the average reward of an optimal and random agent.

### 28/02/24
The results for the combined observation MP were simplified from the results in Mathematica and added to the jupyter notebook.

### 14/03/24
An easier approach to calculate the stationary distribution was found in (Elements of Information Theory, Cover & Thomas).
It uses linear algebra to find the stationary distribution, which is an eigenvector of the transition matrix.
This method is easier to understand that the z transform and was now implemented instead of it.

### 17/03/24
Notation was simplified and made more clear in the first part of the notebook, as well as rudimentary citation.
There is apparently a feature of jupyter allowing bibtex citation, but getting it to work seems not trivial.