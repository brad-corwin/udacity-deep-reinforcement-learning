# Project 1 Report

## Learning Algorithm
This project uses the Deep Q-Network (DQN) algorithm to train an agent to move around an environment and pick up bananas. DQN is built off of the idea of Q-Learning algorithms by utilizing neural networks.

The algorithm has two main parts:
- sample the environment and store the experience in the replay memory
- select a random batch of samples from the memory and learn from them

Naive Q-Learning algorithms learn while practicing. However, the algorithm begins to see correlated effects and the outcome may be swayed by this correlation. ##Experience Replay## helps break the correlation by storing experiences in the replay buffer. These experiences are later randomly sampled during the learning phase.

The DQN algorithm uses two separate neural networks with identical architectures. The target Q-Network is updated less often than the primary Q-Network.

The hyperparamters were initialized the same as written in the [Udacity DQN Agent](https://github.com/udacity/deep-reinforcement-learning/blob/master/dqn/solution/dqn_agent.py). After testing the code against the new environment, the hyperparameters did not need to be changed.

## Plot of Rewards

## Ideas for Future Work
- Change the hyperparameters to see how they effect the algorithms ability to learn.
- Try writing the code using tensorflow.
- Implement the [Rainbow Algorithm](https://arxiv.org/pdf/1710.02298.pdf).
