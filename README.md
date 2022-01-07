# CarRacing-V0_with_PPO

## Introduction
For this project, you will train an car (agent) in a racing environment. 

Reward is -0.1 every frame and +1000/N for every track tile visited, where N is the total number of tiles in track. For example, if you have finished in 732 frames, your reward is 1000 - 0.1*732 = 926.8 points. 

State consists of 96x96 pixels and there is some indicators shown at the bottom of the window for the state of RGB buffer.

The task is episodic and an episode finishes when all tiles are visited. 

CarRacing-v0 defines "solving" as getting average reward of 900 over 100 consecutive trials.

## Getting Started
You need to follow the instructions below to set up your environment :

Clone the repository

```

git clone https://github.com/rym-oualha/CarRacing-V0_with_PPO.git
cd CarRacing-V0_with_PPO
pip install -r requirements.txt

```

## Train the agent 

In order to train the agent you have to:

  1. Initialize the agent

  2. Evaluate state and action space

  3. Train the agent using Proximal Policy Optimization (PPO).

  4. Iterate until agent reaches an average reward of 900 over 100 consecutive trials (over 2500 episodes)

You can train the agent following the instructions in the notebook .ipynb.
