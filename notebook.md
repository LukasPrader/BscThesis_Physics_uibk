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

### 18/03/24
After the next meeting, some notation was again made more clear.

### 19/03/24
A small function calculating the entropy rate for a stationary MP using (Elements of Information Theory, Cover&Thomas) was implemented. It will have to be expanded to be able to use both numerical and symbolic inputs.

### 21/03/24
The stationary MP entropy rate function was improved, also allowing numerical input now.
Another function calculating the block entropy for sequences with given observation probabilities was implemented.
With this, some exploratory plots were made looking at the change in entropy for the MDP and the first two MPs, when changing the light switch probability or the agents policy.

### 23/03/24
An incomplete improvement to the block entropy, making it possible to show the actual block entropy from an initial transition matrix, not only for stationary distributions, has been started.

### 25/03/24
Block entropy was now implemented correctly.
The functions for entropy, entropy rate, stationary distribution and block entropy,
as well as the exploratory plots were moved to a separate notebook for now as to not clutter the old notebook with still largely changing results.

### 01/04/24
An attempt was made to show the block entropy of a biased coin is L*H(p).

### 04/04/24
The results for a general binary system were added, as well as first explanations of the reasons for incompatibility of the entropy ranges for MDP and the observing MPs.

### 05/04/24
Some additional reasoning for the issues regarding model separation was added, as well as the variance of the entropy estimator.

### 07/04/24
Variance of the entropy estimator was set aside, since it is rather complicated,
so the question of confidence was looked at from a sample view point, making use of two sample t-tests.

### 08/04/24
A small addition regarding the model selection idea was made.

### 14/04/24
The block entropy plot was explained in more detail, focussing on the difference of the results to Crutchfield and Feldman.

### 18/04/24
An addition was made, which makes it possible to project block entropy or entropy rate on some (reducing) mapping of the given states.
This now shows correct observations for the entropy rate and block entropy of observing MDP.

A Latex template was created, with one MDP plot done to try out the possibilities in latex.

### 21/04/24
A new document, work_outline.ipynb was created to showcase the current work in a more presentable manner.