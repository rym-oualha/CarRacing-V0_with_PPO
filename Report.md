# Introduction

For this project, you will train an car (agent) in a racing environment from the OpenAI Gym toolkit.
Gym is used for developing and comparing reinforcement learning algorithms.

Reward is -0.1 every frame and +1000/N for every track tile visited, where N is the total number of tiles in track. For example, if you have finished in 732 frames, your reward is 1000 - 0.1*732 = 926.8 points.

State consists of 96x96 pixels and there is some indicators shown at the bottom of the window for the state of RGB buffer.

The task is episodic and an episode finishes when all tiles are visited.

CarRacing-v0 defines "solving" as getting average reward of 900 over 100 consecutive trials.

# Learning Algorithm

<img src="https://github.com/rym-oualha/CarRacing-V0_with_PPO/blob/main/image/ppo%20clip.png?fbclid=IwAR3jx3wnEVaCtAv6biXgtQ6e5oRZVaTqix_TzblHArfSQ40wJDmDtfEYvAk" width="480">

Proximal Policy Optimization, or PPO, is a policy gradient method for reinforcement learning.
