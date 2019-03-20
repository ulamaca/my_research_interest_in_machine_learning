# My Interest in AI and Neuroscience:
My main research interest lies in reinforcement learning and unsupervised learning. I believe that perfect combination of the two can raise the autonomy of machine to a much higer level. My attention is not limited on the hard-core machine learning side but also in its implication in the brain or how inspiration can one get from biological brains on the other way around. Last but not the least, possible applications to technology of this line of research are also very exciting. 
In this repo, I will get all those ideas organized and share relevant information (e.g. papers, tech reports, news...) hope to form a very comprehensive but coherent roadmap showing what my research focu will be in the futrue.

# Resources:

* Latest (Not digested):
    * 2019.03.20: 
        * Tutorial about Transformer (NLP) https://arxiv.org/abs/1903.00374?utm_campaign=Deep%20Learning%20Weekly&utm_medium=email&utm_source=Revue%20newsletter
        * MBRL for Atari (Levine's group) https://sites.google.com/view/modelbasedrlatari/home
        * Blog post on HRL: https://thegradient.pub/the-promise-of-hierarchical-reinforcement-learning/
        * A review for RL for game playing https://arxiv.org/abs/1708.07902
            * great historical summary of development of DQN
    
     

## Reinforcement Learning:
### Research Papers:
* Neuroscience and Psychology:
	* MF and MB RL in the Brain for Control and Decision Making
	* Decision Making Circuitry
    
* Reinforcement Learning
	* Research directions: Multi-Agent Systems, Gradients-Free Methods (Evolution-based), Hyperams Optimization, Bandits, Data Efficiency, Distributed Systems, Architecture Search (AutoML), Curiosity and Exploration, Model-based RL, 
    * [2018 TD3](https://arxiv.org/abs/1802.09477)
        * Top value-based methods in 2018
    * [2018 Soft Actor-Critic](https://arxiv.org/abs/1801.01290)
        * Develop tricks allowing DDPG use stochastic policy
    * [2018 Evolved-PG (Houthooft et al. 2018)](https://arxiv.org/abs/1802.04821),
        * marriage of PG and evolution-based methods, boosting data efficiencey.
    * [2017 MAML (Finn et al. 2017)](https://arxiv.org/abs/1703.03400), [Related Blog by Chelsea Finn, Learning to Learn (2017)](http://bair.berkeley.edu/blog/2017/07/18/learning-to-learn/)
        * Pioneer approach for meta-learning for DRL
    * [2017 Curiosity-driven exploration by self-supervised prediction](https://scholar.google.com/citations?user=AEsPCAUAAAAJ&hl=en#d=gs_md_cita-d&u=%2Fcitations%3Fview_op%3Dview_citation%26hl%3Den%26user%3DAEsPCAUAAAAJ%26citation_for_view%3DAEsPCAUAAAAJ%3A_FxGoFyzp5QC%26tzom%3D-480)
        * ICM module motivates agent to try out unclear part to crave agent's state space. In the end, learned a predictive representation empowering agent to work to some degree without any external supervision.
    * [2017 MADDPG]
        * Using centralized critic to generalize DDPG to general multi-agent setting
    * [2017 PPO]
        * data efficient and easy-to-implement policy gradients agents; also check DeepMind's Parkour agent.

### Resources for Learning:
* Courses:
    * 2018 Udacity DRL Nano-Degree with Github Repo
    * 2018-19 DeepMind/UCL Advanced Deep Learning and Reinforcement Learning
    * 2018-19 OpenAI Spinning Up with Github Repo
    * 2018 UC Berkerley CS294-112 DRL by Sergey Levine
    * 2019 MIT Reinforcement Learning and Control by Dimitri Bertsekas http://web.mit.edu/dimitrib/www/RLbook.html
    * 2015 UCL Reinforcement Learning by David Silver
    * 2018-2019 Intro. to DRL (a survey paper) https://arxiv.org/abs/1811.12560 
    * 2018 Yuxi Li's comprehensive DRL survey (keep updating) https://arxiv.org/abs/1701.07274
    * 2017 Nuts and Bolts of Deep RL Experimentation by John Schulman https://www.youtube.com/watch?v=8EcdaCk9KaQ
    * 2013 Marc Toussant's Bandits, Active Learning, Bayesian RL and Global Optimization https://www.youtube.com/watch?v=5rev-zVx1Ps
* Repos:    
    * Github Repo: RL-Adventure
    * Github Repo: Denny Britz's RL
    * Github Repo: Dopamine (Google's Platform) 
    * Github Repo: PaddlePaddle (Baidu's Platform)
    * Github Repo: OpenAI Baselines 
    * Github Repo: Rich Sutton's Solution, https://github.com/ShangtongZhang/reinforcement-learning-an-introduction
    * Github Repo: Morvan's tutorials, comprehensive materials (programming, DL, RL...)
* Blog Posts:    
    * 2018 Blog Post: alexirpan's RL is not working Yet
    * 2016 Blog Post: Andrej Karpathy's Pong from Pixels     
    * 2017 Blog Post: Otoro's Evolution-based methods, highly visual and interactive http://blog.otoro.net/2017/10/29/visual-evolution-strategies/    
    * 2018 Blog Post: Lessons Learned Reproducing a Deep Reinforcement Learning Paper http://amid.fish/reproducing-deep-rl
    * 2018 Blog Series: Ben Recht, benchmark between PG and random search ttp://www.argmin.net/
    * 2017 Notes: Notes from John Schulman's "Nuts and Bolts of Deep RL Experimentation" lecture https://github.com/williamFalcon/DeepRLHacks
    
## Unsupervised Learning
### Research Papers
* State Representation Learning
	* [State Representation Learning Review (Lesort et al. 2018)](https://arxiv.org/abs/1802.04181)
        * A comprehensive review of state representation learning for control/reinforcement learning.
            
### Resources for Learning:
* Courses:   
    * Video: NIPS 2018 Unsupervised Deep Learning https://www.youtube.com/watch?v=3RVGrz7MjMg
* Blogs Posts:
    * Blog: inFRANCe: https://www.inference.vc/


## Deep Learning in General:
### Resources for Learning:
* Courses:
    * Andrew's Deep Learning Notes
    * Standord's CNN, NLP courses
    * TF Summit 2019 Mar. 
        * TensorFlow 2.0 into https://www.youtube.com/watch?v=k5c-vg4rjBw
* Repos:   
    * David Abel's Summary for Major ML conferences
    * ageron's tf_2 course and hands-on book are great for learning DL programming (using Keras/TF)
    * Udacity's DL_Pytorch, good examples https://github.com/udacity/DL_PyTorch
* Blog Posts:    
    * (RNN) Chris Olah's RNN Tutorial http://colah.github.io/posts/2015-08-Understanding-LSTMs/  
    * (RNN) Andrej Karpathy's RNN simple experiments

## Applications
### Research Papers:
* Healthcare
	* Computational Psychiatry
	* [Learning Representations for Counterfactual Inference (Johansson et al 2016)](https://arxiv.org/abs/1605.03661)
        * Counter-factual inference in the context of healthcare; using Deep learning models.

### Resources for Learning:
* Courses:
    * [Reinforcement Learning in Healthcare: Challenges and Promise (Video by Finale Doshi-Velez, 2018)](https://www.youtube.com/watch?v=OsGxPVYR2xo)
