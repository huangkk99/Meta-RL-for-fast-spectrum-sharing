# Meta-RL-for-fast-spectrum-sharing

The corresponding paper for this project is K. Huang, L. Liang, S. Jin, and G. Y. Li, "Meta reinforcement learning for fast spectrum sharing in vehicular networks", arxiv preprint:2309.17185, Sep. 2023.  

Requirement: Python > 3.6, torch > 1.4.0

Environment_marl: The environment of a single task for learning from scratch or fine tuning.  
Environment_meta: The environment, of which the five key factors can be changed to generate different tasks.  
sarltrain_ppo: The training code for a single task. It can be used to learn from scratch and fine-tune the meta parameters.  
metatrain_ppo_test: The code for meta training.

The whole process:
1. Run the metatrain_ppo_test.py to obtain the meta parameters, 2. Use the meta parameters as the initialization to adapt them to the new environment.
