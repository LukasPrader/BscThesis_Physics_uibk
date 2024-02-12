This file serves as a kind of "lab book" documenting my working process.

### 09/02/24
Up until now, my progress consisted of trying to familiarize myself with some concepts from (Crutchfield & Feldmann 2001), implementing an approximation of the entropy of a fair coin flip with an increasing amount of data.
Today, an analysis on the MDP shown in "Affordance-based-PS-demo.ipynb" was done by looking at Markov processes (MPs) resulting from only observing the system.
One can create three different MPs, one only observing the state of the light, one only observing the rat's actions, and one observing both. When observing both, one has to choose how exactly the light state and action state are connected. I decided to look at combined states resulting from the current state of the light, and the action that was just performed to bring the system to that state.
One can then calculate the probabilities of each respective state of the mentioned MPs occurring, as shown in "first_steps.ipynb".

### 11/02/24
The graphs and calculations were now put into the jupyter notebook from handwritten notes, now also including the probability for the light turning on.
