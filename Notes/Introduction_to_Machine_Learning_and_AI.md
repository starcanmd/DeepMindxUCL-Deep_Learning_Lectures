# Introduction to Machine Learning & AI (1/12) #

**Instructor:** Professor Thore Graepel, DeepMind Research Scientist and UCL Chair of Machine Learning

**Total Length:** 1 hr 25 min 18 ms

Plan of the Lecture:

* Solving Intelligence

* AlphaGo & AlphaZero

* Learning to Play Capture the Flag

* Folding Proteins with AlphaFold

* Overview of Lecture Series

## Solving Intelligence ##

The hallmark of human intelligence is its generality, the ability to do a wide range of things well. Best expressed by Robert A. Heinlein:

'A human being should be able to change a diaper, plan an invasion, butcher a hog, conn a ship, design a building, write a sonnet, balance accounts, build a wall,set a bone, comfort the dying, take orders, give orders,cooperate, act alone, solve equations, analyze a new problem, pitch manure, program a computer, cook a tasty meal, fight efficiently, die gallantly. Specialization is for insects.'

Shane Legg's definition of intelligence:

Intelligence measures an agent's ability to achieve goals in a wide range of environments. His formal theory is:

<img src="/Images/Intro_1.png" width=500 height=300>

Measure of intelligence is a function of pi -a policy-. 

A policy determines what action to take in a given state.

This measure of intelligence is expressed as sum over all computable environments. This term represents breadth of all the things that an intelligent agent should be able to do.

Check algorithmic information theory.

Indication of success = Value achieved (the value that policy pi creates in environment mu)

Complexity penalty: A weighting term. K of mu is the Kolmogorov complexity of the environment mu. If the complexity is low, this term will be great. Therefore, it gives more weight to simpler environments and progressively less weight to more complex ones. Since there are more complex environments than simple ones, it also acts as a normalization.

Policy and value comes from * Reinforcement Learning *

There is an agent that interacts with an environment which poses a task or problem. Agent observes the state of the environment and then take an action and influence its environment. After the action, it receives subsequent observation what has happened as a consequence and it receives a reward. 

The goal of the agent is to learn a policy, pi, to maximize long-term reward.

Why does DeepMind work on games?

* Microcosms of the real world: * Ground for real-world situations.

* Stimulate intelligence: * A diverse set of challenges.

* Good to test in simulations: * Large scale simulations. Thousands in parallel, faster than real life.

* Measure progress and performance: * Comparability against human performance.

In deep reinforcement learning, the policy is parameterised by a neural network whose parameters we are trying to adapt for long-term success.

### Role of Deep Learning: ###

* Enable end-to-end learning: Put the raw features and learn the desired input-output mapping. Just need the loss, how you measure the success, and the architecture of the neural network. 

* We can put our prior knowledge into solution of our problem, making learning easier by less computing power and training data.

* Greater computational power (GPUs, TPUs), more available data, better understanding of algorithms and architectures

## AlphaGo and AlphaZero ##
