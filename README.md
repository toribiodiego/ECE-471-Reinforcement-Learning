

> This repository contains the code for **ECE471: Reinforcement Learning**, a 3-credit graduate-level course at The Cooper Union for the Advancement of Science and Art, exploring core reinforcement learning principles through rigorous study and practical programming assignments.


## Reinforcement Learning
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


### Repository Structure

```
.
├── Final_Project
│   ├── Final_Project_Report.pdf
│   └── README.md
├── P01
│   └── P01.ipynb
├── P02
│   └── P02.ipynb
├── P03
│   ├── P03.ipynb
│   ├── PS03_Report.pdf
│   └── README.md
└── README.md
```

- **`P01.ipynb`** – *Programming Assignment 1*  
  -  Introduces the fundamentals of reinforcement learning through multi-armed bandit problems using epsilon-greedy strategies and reward updating.

- **`P02.ipynb`** – *Programming Assignment 2*  
  - Develops a custom racetrack environment to explore agent behavior and policy evaluation via off-policy Monte Carlo methods.

- **`P03.ipynb`** – *Programming Assignment 3*  
  - Explores on-policy methods within a simulated Markov Decision Process framework, examining performance trade-offs and convergence through various update strategies.

- **`Final_Project.ipynb`** – *RL Self-Play Agent for Checkers using PPO*  
  - Demonstrates a deep reinforcement learning approach using self-play and an enhanced PPO framework, with detailed performance analysis in the accompanying report.



### Final Project

The project, *Checkers Agent via Self-Play and Proximal Policy Optimization (PPO)*, focuses on creating a reinforcement learning agent capable of mastering Checkers exclusively via self-play, utilizing the PPO framework initially described in the original [PPO](https://arxiv.org/pdf/1707.06347) paper. Initially, we validated our PPO implementation on benchmark environments such as CartPole and Lunar Landing to ensure correctness and efficiency. Next, we demonstrated its effectiveness by extending it to Tic-Tac-Toe, confirming that our agent could learn strategic gameplay through self-play. Ultimately, we successfully trained an agent to play Checkers, showcasing clear strategic improvements against random opponents. Through this process, we developed a systematic approach to applying deep reinforcement learning methodologies to domains where these techniques are less commonly explored.