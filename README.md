# DeepRL-Continuous_Control
2-DoF Robot Arm Control Agent. Udacity Deep Reinforcement Learning Nanodegree 2nd Project.

## Project overview 
In this project we implement a reinforcement learning agent using [Deep Deterministic Policy Gradients (DDPG)](https://arxiv.org/abs/1509.02971) algorithm. The agent is required to learn the how to control a double-jointed arm so that it can move to target locations. The world environment, where the arm moves, is based on [Unity ML-agents](https://github.com/Unity-Technologies/ml-agents) and the environment looks as in the figure below.

![img_1](Figures/reacher.gif)

## Environment details 
The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

To learn the optimal policy, a reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The task is episodic, and in order to solve the environment:
- Version 1: the agent must get an average score of +30 over 100 consecutive episodes.
- Version 2: the agents must get an average score of +30 (over 100 consecutive episodes, and over all agents)

## Instalation and Running 

1. Configure a Python 3.6 / PyTorch 0.4.0 environment with the needed requirements as described in the [Udacity repository](https://github.com/udacity/deep-reinforcement-learning#dependencies)

2. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Version 1: one agent
      - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
      - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
      - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
      - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)
    - Version 2: twenty agents
      - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
      - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
      - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
      - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)
      
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.
    
    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use this [link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip) (version 1) or this [link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux_NoVis.zip) (version 2) to obtain the "headless" version of the environment. You will not be able to watch the agent without enabling a virtual screen, but you will be able to train the agent. (To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the Linux operating system above.)
  
3. Download the `Continuous_Control.ipynb`, `model.py` and `ddpg_agent.py` files in the DeepRL-Navigation GitHub repository and make them accessible to your python environment.   

## Trining 
Execute the provided notebook within Deep Reinforcement Learning Udacity online workspace for navigation project after modifying `Continuous_Control.ipynb` and related files.
