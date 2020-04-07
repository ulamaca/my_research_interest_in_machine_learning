## Format:
* Method Name:    
    * Key Features:
        * ML-Type: Supervised/Unsupervised/Reinforcement
        * ML-Subtype: (Supervised/Unsupervised) Few Shots, (Unsupervised) Self-supervised, (Reinforcement) Imitation, Reverse RL
    * Arch-Type: Neural Networks, Linear Model, CNN, ...
    * Short Idea: 
    * Resources: 
    * (optional) Usecases
    
    
## (short) Machine Learning Zoo
* Self Organizing Maps (SOM):
    * Key Features: Unsupervised, Topology-Preserving, Neuro-Inspired (Sensory Cortex, Central Excitation vs Lateral Inhibition), Auto #Cluster Determination
    * Arch-Type: NN (2-layer)
    * Short Idea: using standard NN training scheme to learn a set (usually 2-D and can be N-D) of neurons that preserve the spatial relation. Each active neuron will be a cluster center. Objective: competition-cooperation-adaptation.    
    * Resources:
        * [An illustrative short intro. (by Thales Sehn Körting)](https://www.youtube.com/watch?v=H9H6s-x-0YE)      
        * Implementations: [MiniSOM](https://github.com/JustGlowing/minisom), [SOMPY](https://github.com/sevamoo/SOMPY), [SimpSOM](https://github.com/fcomitani/SimpSOM)
    * Usecases:
        * Deriving reward function for plausible structure, novelty for molecule generation. (Nature Biotech 2019)  

* Inverse Reinforcement Learning
    * Key Features: Reinforcement Learning/Supervised Learning, Learning Reward Function from Policy (Reverse), Imitation Learning
    * Short Idea: to learn rewards from expert (and them reinforcement-learn from it)
    * Usecases:
        * research: GAIL (2016)

* ELBO (Evidence Lower BOund; aka Evidence Lower Bound)
    * Evidence = likelihood
    * Marginal Evidence

* Variance in Reinforcement Learning setting
    * [reference](https://medium.com/mlreview/making-sense-of-the-bias-variance-trade-off-in-deep-reinforcement-learning-79cf1e83d565)

        
## Glossary
* Topology: geometric properties or spatial relation or arrangement/order that will not be changed by (continuous) deformation of the subject.