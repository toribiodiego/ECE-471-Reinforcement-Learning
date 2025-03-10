


> This repository contains code for **ECE471: Reinforcement Learning (Independent Study, Fall 2024)**, a 3-credit graduate course conducted as an independent study under the guidance of **Professor Chris Curro**. Weekly meetings were held to discuss textbook readings from *Reinforcement Learning: An Introduction* by Sutton & Barto (2018), while practical programming assignments provided hands-on experience with foundational RL concepts.


## Course Overview

This course offers a comprehensive introduction to reinforcement learning by covering key topics such as Markov Decision Processes, dynamic programming, Monte Carlo methods, temporal-difference learning, and function approximation. Both model-based and model-free RL algorithms are examined through theoretical discussions and practical assignments. The curriculum emphasizes the design and implementation of RL agents capable of learning and adapting in complex environments.

## Codebase Structure

- **P01** – *Programming Assignment 1*  
  Implements multi-armed bandit algorithms to RL fundamental concepts such as epsilon-greedy action selection and reward updating methods. This assignment establishes the groundwork for understanding action-value estimation and the balance between exploration and exploitation.

- **P02** – *Programming Assignment 2*  
  Features a custom racetrack environment that simulates a realistic driving scenario. This assignment focuses on developing an environment, defining agent behavior, and applying *off-policy Monte Carlo* methods for policy evaluation and trajectory visualization.

- **P03** – *Programming Assignment 3*  
  Examines reinforcement learning in simulated Markov Decision Process settings. It includes both on-policy and uniform update strategies to evaluate performance convergence and stability through policy evaluation techniques, highlighting the interplay between exploration and exploitation.

- **Final_Project** – *RL Self-Play Agent for Checkers using PPO*  
    Includes a detailed report and implementation of a deep reinforcement learning agent for Checkers. The agent is trained solely via self-play using an enhanced Proximal Policy Optimization (PPO) framework. Key improvements include orthogonal weight initialization, a custom Adam optimizer with an adjusted epsilon, Generalized Advantage Estimation (GAE), mini-batch updates, normalized advantages, clipped surrogate objectives, and global gradient clipping. Performance evaluations demonstrate the agent's ability to learn ~~and master~~ Checkers through self-play.


## Final Project

