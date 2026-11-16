# Where Does Kinesin stall? - A minimal stochastic model of a molecular motor under load.

## Research question
> ** How does a minimal stochastic model of kinesin respond to increasing cargo load and what determines when it stalls?

The project split this research question into 3 subquestions:
1, Can a minimal stochastic model reproduce the slowing down and stalling of kinesin that is seen in experiments?
2, Which ingredients does the model need in order to stall?
3, How do the model assumptions and parameters shift the predicted stall force?

## Abstract
A Kinesin-1 is a molecular motor that is using ATP hydrolysis in order to transport cargo along microtubules in 8 nm steps. Experiments have shown that the kinesin slows down under increased cargo load and eventually reaching a stalling state meaning that there is no forward motion. This ask therefore the question when this state appears, what is the causing parameters and whether or not it can be modelled through a simple stochastic dynamics system. 

Ariga et al research lays the foundation for the project where they used a two state markov stepping model in order to determine where the energy is going under this transportation. The forward and backward steps was modelled through Bell's law and the trajaectory is simulated with Gillespie algorithm. Nulling the load yields a force velocity cure and stall gorces which are checked against the analytical steady-state solution and comapred with the experimaental results. Note that the steady state solution is not a stalling state since the Kinesin consume ATP even when taking steps backwards. 
The method will involve reducing the load and backward steps in order to determine which one is needed to a stalling state. The model parameters will also vary to understand how they affect the stall force. 
