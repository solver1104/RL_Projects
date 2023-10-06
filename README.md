# RL_Projects
This repo contains a few of my Reinforcement Learning projects. I have implemented and trained 3 RL algorithms on 3 different control tasks. Trained weights for these tasks are provided alongside the models.

## SAC
This folder contains an implementation for the Soft Actor-Critic method and trained weights for it to play OpenAI Gym's CarRacing environment. The agent learns to play a simple racing game from the pixels of the game, and is rewarded for driving the track faster. The track is randomized at the beginning of each iteration, so the agent must learn a robust policy that can drive effectively in multiple track layouts. It achieves an average score of 907 after training, surpassing the 900 threshold for "solving" the environment.

### Trained Model Demonstration
![SAC Demonstration](https://github.com/solver1104/RL_Projects/blob/main/CarRacing_SAC_Demonstration.gif)

## TD3

This folder contains an implementation for the Twin Delayed DDPG (TD3) algorithm and trained weights for OpenAI Gym's BipedalWalker environment. The humanoid agent learns to walk on uneven terrain by controlling its joints while minimizing the energy used to do so. It achieves a consistent score of 312 after training, surpassing the 300 threshold for "solving" the environment.

### Trained Model Demonstration
![TD3 Demonstration](https://github.com/solver1104/RL_Projects/blob/main/BipedalWalker_TD3_Demonstration.gif)

## DQN
This folder contains an implementation for a Deep Q Network and trained weights for OpenAI Gym's CartPole environment, one of the most well known control environments for RL. The agent learns to balance a vertical pole on top of a movable cart and achieves the maximum reward possible for this environment (500). This implementation makes use of the Experience Replay, Double Q, and Dueling DQN modifications to the original DQN architecture to stabilize training.

### Trained Model Demonstration
![DQN Demonstration](https://github.com/solver1104/RL_Projects/blob/main/CartPole_DQN_Demonstration.gif)