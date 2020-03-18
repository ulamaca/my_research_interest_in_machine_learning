# Miscellaneous Resources:

# Resources:

* Latest (Not digested):
    * 2019.03.25: 
        * 1 Tutorial about Transformer (NLP) https://arxiv.org/abs/1903.00374?utm_campaign=Deep%20Learning%20Weekly&utm_medium=email&utm_source=Revue%20newsletter     
        * https://towardsdatascience.com/checklist-for-debugging-neural-networks-d8b2a9434f21
	* TF dev summit (check TF's medium) 
    * TF2, the tutorial from ageron
    
     

## Reinforcement Learning:
### Research Papers:
* Neuroscience and Psychology:
	* MF and MB RL in the Brain for Control and Decision Making
	* Decision Making Circuitry
    
* Reinforcement Learning
	* Research directions: Multi-Agent Systems, Gradients-Free Methods (Evolution-based), Hyperams Optimization, Bandits, Data Efficiency, Distributed Systems, Architecture Search (AutoML), Curiosity and Exploration, Model-based RL, 
    * [MBRL for Atari (Lukasz Kaiser et al. 2019)](https://sites.google.com/view/modelbasedrlatari/home)
        - extend world models (Ha et al. 2018) into Atari environment, and achieved 10x steps sample efficiency.
        - technical:
            - world model is using E-D arch (like Oh's 2015) with several tricks: 1. skipped connections, like Ladder networks, 2. influences of action embedding on all decoding layers, 3. discrete representation (from other 2018 work) to prevent temporal prediction error accumulation, 4. stochastic models has a reccurrent module work as q-sampling mechanism in VAE. ; 3. esp. 4. can be studied in more details.
        - one source of stochasisity of Atari comes from frame stacking (consecutive previous 4 frames) will miss effect of certain actions such as pause which lasts more than 4 frames.
        - some inspiration for building dynamic latent models; I am always thinking the decoding part can be removed, probably something can be done with skipped connection tricks.           
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
    * 2018 [Deep Learning for Video Game Playing](https://arxiv.org/abs/1708.07902)
        * great historical summary of development of DQN, specialized for game playing applications
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
    * 2019 Blog post on HRL: https://thegradient.pub/the-promise-of-hierarchical-reinforcement-learning/
        - concept: decompose the tasks into pretinent granularity, then solve subtasks, in the end solve the main in the end.
        - four fundamental approaches: 1. Feudal networks (manager-worker sysmems), 2. options framework, 3. HAM, finite state transition models with states abstract from env/agent information can be context (for states) and pre-designed options (for action executions), 4. MaxQ: tree representation
            - A summary for proper situations for each methods mentioned    
        - list recent works to extend these approaches with DNNs
    
## Unsupervised Learning
### Research Papers
* State Representation Learning
	* [State Representation Learning Review (Lesort et al. 2018)](https://arxiv.org/abs/1802.04181)
        * A comprehensive review of state representation learning for control/reinforcement learning.
* [my own master thesis](https://drive.google.com/file/d/1wRXt6PFYZ2QVWhvixJ_ZYiXbfG4QE41b/view), Chapter 2 summarizes representatation learning and autoencoders:
   
            
### Resources for Learning:
* Courses:   
    * Video: NIPS 2018 Unsupervised Deep Learning https://www.youtube.com/watch?v=3RVGrz7MjMg
* Blogs:
    * inFRANCe: https://www.inference.vc/
    * [Lil's Log (a good site for DL/RL and other related topics)](https://lilianweng.github.io/lil-log/2020/01/29/curriculum-for-reinforcement-learning.html?utm_campaign=NLP%20News&utm_medium=email&utm_source=Revue%20newsletter#curriculum-through-distillation)


## Deep Learning in General:
### Resources for Learning:
* Courses:
    * Andrew Ng's Deep Learning Notes (from Tez)
    * Andrew Ng's Deep Learning Yearning
    * Standord's CNN, NLP courses
    * TF Summit 2019 Mar. 
        * TensorFlow 2.0 into https://www.youtube.com/watch?v=k5c-vg4rjBw
    * PyTorhc, TF dictionary (for searching for useful command): https://www.aiworkbox.com/lessons
* Repos:   
    * David Abel's Summary for Major ML conferences
    * ageron's tf_2 course and hands-on book are great for learning DL programming (using Keras/TF)
	* http://www.10tiao.com/html/511/201903/2652040568/4.html his talk in chinese
    * Udacity's DL_Pytorch, good examples https://github.com/udacity/DL_PyTorch
* Blog Posts:    
    * (RNN) Chris Olah's RNN Tutorial http://colah.github.io/posts/2015-08-Understanding-LSTMs/  
    * (RNN) Andrej Karpathy's RNN simple experiments
    * [2019 (Classification)分类性能度量指标：ROC曲线、AUC值、正确率、召回率、敏感度、特异度](https://blog.csdn.net/miao0967020148/article/details/88583824)

## Applications
### Research Papers:
* Healthcare
	* Computational Psychiatry
	* [Learning Representations for Counterfactual Inference (Johansson et al 2016)](https://arxiv.org/abs/1605.03661)
        * Counter-factual inference in the context of healthcare; using Deep learning models.

### Resources for Learning:
* Courses:
    * [Reinforcement Learning in Healthcare: Challenges and Promise (Video by Finale Doshi-Velez, 2018)](https://www.youtube.com/watch?v=OsGxPVYR2xo)
