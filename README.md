

> This repository contains the code for **ECE471: Reinforcement Learning**, a 3-credit graduate-level course at The Cooper Union for the Advancement of Science and Art, exploring core reinforcement learning principles through rigorous study and practical programming assignments.


## Experimentation with PyTorch
**Independent Study, Fall 2024**  
**Instructor:** Professor Chris Curro

### Overview

This independent study provides a practical introduction to reinforcement learning by exploring core topics such as Markov Decision Processes, dynamic programming, Monte Carlo methods, and temporal-difference learning. Through structured discussions, targeted programming assignments, and a comprehensive final project, students build the theoretical foundations and practical expertise needed to develop RL agents that can learn and adapt in complex environments.

### Material

The primary resource for this course is the textbook [*Reinforcement Learning: An Introduction*](https://www.goodreads.com/book/show/42601538-reinforcement-learning) by Sutton & Barto (2018), which covers:

- Modeling and solving Markov Decision Processes
- Dynamic programming techniques
- Monte Carlo methods for policy evaluation
- Temporal-difference learning and function approximation


## Repository Structure

- **P01** – *Programming Assignment 1*  
  Implements multi-armed bandit algorithms to RL fundamental concepts such as epsilon-greedy action selection and reward updating methods. This assignment establishes the groundwork for understanding action-value estimation and the balance between exploration and exploitation.

- **P02** – *Programming Assignment 2*  
  Features a custom racetrack environment that simulates a realistic driving scenario. This assignment focuses on developing an environment, defining agent behavior, and applying *off-policy Monte Carlo* methods for policy evaluation and trajectory visualization.

- **P03** – *Programming Assignment 3*  
  Examines reinforcement learning in simulated Markov Decision Process settings. It includes both on-policy and uniform update strategies to evaluate performance convergence and stability through policy evaluation techniques, highlighting the interplay between exploration and exploitation.

- **Final_Project** – *RL Self-Play Agent for Checkers using PPO*  
    Includes a detailed report and implementation of a deep reinforcement learning agent for Checkers. The agent is trained solely via self-play using an enhanced Proximal Policy Optimization (PPO) framework. Key improvements include orthogonal weight initialization, a custom Adam optimizer with an adjusted epsilon, Generalized Advantage Estimation (GAE), mini-batch updates, normalized advantages, clipped surrogate objectives, and global gradient clipping. Performance evaluations demonstrate the agent's ability to learn ~~and master~~ Checkers through self-play.


## Final Project

