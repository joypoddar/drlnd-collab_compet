[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135623-e770e354-7d12-11e8-998d-29fc74429ca2.gif "Trained Agent"
[image2]: https://user-images.githubusercontent.com/10624937/42135622-e55fb586-7d12-11e8-8a54-3c31da15a90a.gif "Soccer"


# Project 3: Collaboration and Competition

### Introduction

For this project, you will work with the [Tennis](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis) environment.

![Trained Agent][image1]


In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1.  If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01.  Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation.  Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping. 

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

- After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.
- This yields a single **score** for each episode.

The environment is considered solved, when the average (over 100 episodes) of those **scores** is at least +0.5.

### Getting Started

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux_NoVis.zip) to obtain the "headless" version of the environment.  You will **not** be able to watch the agent without enabling a virtual screen, but you will be able to train the agent.  (_To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)

2. Make sure you have downloaded and installed Anaconda. You can download it from https://www.anaconda.com/distribution/

3. Now you can create your environment. Since this environment refers to a Udacity project for the Deep Reinforcement Learning Nanodegree, lets call our environment `DRLND`.

    Linux or Mac:
    ```sh
    conda create --name drlnd python=3.6
    source activate drlnd
    ```
    
    Windows:
    ```sh
    conda create --name drlnd python=3.6 
    activate drlnd
    ```
    
    
4. We will be working with pytorch version 0.4.0 (an early version), so make sure that you install this version of pytorch first by typing:
    ```sh
    conda install pytorch=0.4.0 -c pytorch
    ```
    
5. Perform a minimal installation of the OpenAI Gym environment (see instructions here: https://github.com/openai/gym)

6. For the rest of the prerequisities please do type:
    ```sh
    pip install .
     ```
     The above line of code assumes that at the folder you are working, you have the `setup.py` which includes the UnityAgents and the `requirements.txt` file that contains other useful packages (that exist in that repository).
     
7. Create a Python execution backend for Jupyter for the drlnd environment
    ```sh
    python -m ipykernel install --user --name drlnd --display-name "drlnd"
    ```
     
Now you are not only ready to use the UnityAgents evnironment, but the OpenAI Gym as well.  You are all set to start playing with reinforcement learning environments! Yay!

Other useful utilities will also be installed if you follow these directions, including Jupyter Notebook, so consider the above installation guide as a complete guide to setup your RL environments!

### Instructions

Follow the instructions in `Tennis.ipynb` to get started with training your own agent!  

### Report

There is a file named **Report.ipynb** which has detailed description of the code and its workings.
