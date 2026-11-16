# Where Does Kinesin stall? - A minimal stochastic model of a molecular motor under load.

## Research question
> **How does a minimal stochastic model of kinesin respond to increasing cargo load, and what determines where it stalls?**

The project split this research question into 3 subquestions:
1. Can a minimal stochastic model reproduce the slowing down and stalling of kinesin that is seen in experiments?
2. Which ingredients does the model need in order to stall?
3. How do the model assumptions and parameters shift the predicted stall force?

## Abstract
Kinesin-1 is a molecular motor that uses ATP hydrolysis to transport cargo along microtubules in 8 nm steps. Experiments have shown that kinesin slows down as the cargo load increases and eventually stalls at roughly 7 pN, where there is no net forward motion [2]. This project asks at what load the stall occurs, which parameters determine it, and whether it can be captured by a minimal stochastic model. 

The project builds on Ariga et al. [1], who described kinesin as a two-state Markov stepper in which the forward and backward steps depend on the load through Bell’s law. Here, trajectories of this model are simulated with the Gillespie algorithm [5]. Increasing the load step by step yields a force–velocity curve and a stall force, which are checked against the analytical steady-state solution and compared with experimental results [2, 3]. To identify which ingredients are needed for stalling, backward steps and the load-independent chemical step are removed one at a time, and the model parameters are varied to show how they shift the stall force.

## Background
Kinesin-1 walks hand-over-hand along a microtubule and advances 8 nm for each ATP molecule it hydrolyses [2]. When an opposing load is applied, for example with an optical trap that pulls the cargo backwards [1, 2], the motor slows down and takes backward steps more often [3]. At the stall force, forward and backward steps occur at equal rates, so there is no net motion. Simple discrete-state stochastic models have been shown to describe such force–velocity measurements well [4]. This project uses the two-state model of Ariga et al. [1] as a starting point and investigates which of its ingredients (the load-dependent stepping rates, the backward steps and the load-independent chemical step) are responsible for the stall.

## Method
