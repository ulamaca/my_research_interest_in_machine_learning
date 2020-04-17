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
    * Evidence = (Marginal) likelihood P(X) X is the observed dataset

* Variance in Reinforcement Learning setting
    * it is the variance of Total reward over trajectory; so it is a expectation over policy distribution and through reward transform 
    * [reference](https://medium.com/mlreview/making-sense-of-the-bias-variance-trade-off-in-deep-reinforcement-learning-79cf1e83d565)

* ANOVA (ANalysis of VAriance)
    * Goal: to test 1 factor with multiple groups (conditions), whether there is at least one group has significant difference (but not knowing which specific one differs)
    * Short Idea: Signal/Noise ratio test (using F-statistics); *Signal*=between group variance (MSG) and *Noise*=average within group variance (MSE) 
    * Usecases: 
        * example question: Are these brands ACER/DELL/ASUS/Apple having different battery duration? 
    * Roadmap: T-test (1 factor, 2 groups) -> ANOVA (1 factor, N groups, test: any difference?) -> multiple T-Tests (1 factor, N groups, test: where is the difference?)

        
## Glossary
* Topology: geometric properties or spatial relation or arrangement/order that will not be changed by (continuous) deformation of the subject.