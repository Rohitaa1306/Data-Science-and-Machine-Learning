# Reinforcement Learning for CartPole

This repository contains Python code implementing a reinforcement learning solution for the CartPole-v1 environment using TensorFlow and OpenAI Gym.

## Overview

Reinforcement learning is a type of machine learning where an agent learns to make decisions by interacting with an environment. In this project, we use reinforcement learning to train an agent to balance a pole on a moving cart in the CartPole-v1 environment.

## Details

Environment Setup: The code uses the CartPole-v1 environment from OpenAI Gym, setting up the state and action spaces.

Q-Learning Parameters: Hyperparameters like learning rate, discount factor, and exploration rate are defined for the Q-learning algorithm.

Q-Network: A neural network (Q-network) is implemented using TensorFlow's Keras API, with layers for input, hidden, and output.

Training Loop: The agent interacts with the environment over multiple episodes, balancing exploration and exploitation.

Experience Replay: Experiences are stored in a replay memory, and the agent is trained using a stochastic gradient descent approach.

Visualization: Training progress is visualized through a plot of total rewards over episodes.

## Results
Training progress, including average rewards and exploration rates, is printed during the script execution.

The script generates a plot showing the learning curve of total rewards over episodes.

Average test reward is printed at the end of training to evaluate the agent's performance.
