# Q-learning, Dyna-Q, and Mutated Versions

## Overview
This Jupyter Notebook explores the implementation of Q-learning and Dyna-Q algorithms in reinforcement learning, specifically applied to the "CartPole-v1" environment from OpenAI's Gym. The notebook demonstrates the differences in performance and efficiency between the two algorithms through various visualizations and analyses.

## Table of Contents
1. [Introduction](#introduction)
2. [Import Libraries and Initialize Environment](#import-libraries-and-initialize-environment)
3. [Discretize State Space](#discretize-state-space)
4. [Implement Q-learning](#implement-q-learning)
5. [Implement Dyna-Q](#implement-dyna-q)
6. [Training and Evaluation](#training-and-evaluation)
7. [Comparative Analysis](#comparative-analysis)
8. [Visualizations](#visualizations)
9. [Conclusion](#conclusion)

## Introduction
Reinforcement learning (RL) is a type of machine learning where an agent learns to make decisions by taking actions in an environment to maximize cumulative rewards. This notebook focuses on two popular RL algorithms: Q-learning, a model-free algorithm, and Dyna-Q, which combines model-free and model-based approaches.

## Import Libraries and Initialize Environment
In this section, we import the necessary libraries and initialize the "CartPole-v1" environment. The environment simulates a cart with a pole attached to it, and the goal is to balance the pole by moving the cart left or right.

### Key Libraries Used:
- `gym`: For creating and managing the environment.
- `numpy`: For numerical operations.
- `matplotlib`: For visualizations.

## Discretize State Space
Since the state space of the "CartPole-v1" environment is continuous, we discretize it into bins to make it manageable for the Q-learning algorithm. This section defines the bins for cart position, cart velocity, pole angle, and pole angular velocity.

## Implement Q-learning
This section details the implementation of the Q-learning algorithm, including the update rules and the training process. The Q-table is initialized, and the agent learns to balance the pole through exploration and exploitation.

## Implement Dyna-Q
Dyna-Q enhances Q-learning by incorporating a model of the environment. This section describes how Dyna-Q uses simulated experiences to improve learning efficiency.

## Training and Evaluation
In this section, both Q-learning and Dyna-Q are trained on the same task. The performance of each algorithm is evaluated based on the rewards obtained during training.

## Comparative Analysis
This section compares the performance of Q-learning and Dyna-Q through various metrics, including:
- Average rewards over episodes
- Learning efficiency
- Convergence speed

## Visualizations
Several plots are generated to visualize the results:
- **Reward Histograms**: Comparing the reward distributions of Q-learning and Dyna-Q.
- **Reward Difference Plot**: Showing the difference in rewards between the two algorithms.
- **Cumulative Reward Plot**: Illustrating the cumulative rewards over episodes for both algorithms.

## Conclusion
The notebook concludes with a summary of findings, highlighting the advantages of Dyna-Q over Q-learning in terms of efficiency and effectiveness in learning.

## Usage
To run this notebook:
1. Ensure you have Python 3 and the required libraries installed.
2. Open the notebook in Jupyter or Google Colab.
3. Execute the cells sequentially to observe the training and results.

## Requirements
- Python 3.x
- Libraries: `gym`, `numpy`, `matplotlib`, `scipy`

## Acknowledgments
This notebook utilizes the OpenAI Gym library for the environment and is inspired by various reinforcement learning resources and research papers.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
