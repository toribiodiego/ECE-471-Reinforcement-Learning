# Proximal Policy Optimization with Self-Play: Training Strategic Checkers Agents

## Project Overview

This project implements and evaluates a Proximal Policy Optimization (PPO) algorithm enhanced with various modifications for stability and efficiency, specifically applied to training reinforcement learning agents to play CartPole, Tic-Tac-Toe, and Checkers. The core aim was to explore self-play dynamics and evaluate the performance improvements from specific PPO enhancements.

---

## Files in the Repository

- **Final_Project.ipynb**: Contains the complete code implementation, from PPO training to evaluation.
- **Final_Project_Presentation.pdf**: Slides summarizing the project approach, methodology, and key results.
- **Final_Project_Report.pdf**: Comprehensive report detailing methods, experiments, results, and analysis.


## Project Overview

This project implements and evaluates a Proximal Policy Optimization (PPO) algorithm enhanced with various modifications for stability and efficiency, specifically applied to training reinforcement learning agents to play CartPole, Tic-Tac-Toe, and Checkers. The core aim was to explore self-play dynamics and evaluate the performance improvements from specific PPO enhancements.

---

## Files in the Repository

- **Final_Project.ipynb**: Contains the complete code implementation, from PPO training to evaluation.
- **Final_Project_Report.pdf**: Comprehensive report detailing methods, experiments, results, and analysis.

---

## Methodology

The project expands upon the baseline PPO algorithm with several enhancements:

### PPO Enhancements:
- **Orthogonal Initialization**: Stabilizes learning through improved gradient flow.
- **Custom Adam Optimizer**: Adjusted epsilon parameter for numerical stability.
- **Generalized Advantage Estimation (GAE)**: Smooths advantage estimates, balancing bias and variance.
- **Mini-Batch Updates**: Improves training stability and reduces catastrophic policy updates.
- **Advantage Normalization**: Keeps the policy updates consistent and numerically stable.
- **Clipped Surrogate Objective**: Prevents large policy deviations, enhancing PPO stability.
- **Value Function Loss Clipping**: Avoids large, destabilizing updates in value predictions.
- **Entropy Bonus**: Encourages sustained exploration throughout training.
- **Global Gradient Clipping**: Protects against exploding gradients.
- **Separate Actor and Critic Networks**: Prevents interference, optimizing performance for complex environments.

---

## Results

### CartPole-v1
The enhanced PPO implementation successfully achieved stable and optimal performance:
- **Episodic Return**: Consistently exceeded 400, demonstrating effective learning and convergence.
- **Entropy Loss**: Decreased gradually, indicating successful exploration-to-exploitation transition.
- **Value and Policy Loss**: Showed steady convergence, validating stable training dynamics.

### Tic-Tac-Toe
Performance improved significantly with training:

<div align="center">

| Checkpoint | Agent Move Order | Wins | Losses | Draws |
|------------|------------------|------|--------|-------|
| Random     | First            | 597  | 268    | 135   |
| Easy       | First            | 680  | 225    | 95    |
| Easy       | Second           | 290  | 636    | 74    |
| Medium     | First            | 775  | 178    | 47    |
| Medium     | Second           | 439  | 543    | 18    |
</div>


<br>
- Agent demonstrated increased strategic play when moving first.
- Performance against opponents improved consistently across checkpoints.
- Agent improved but still struggled significantly when moving second.

### Checkers
Notable strategic development was observed:

<div align="center">

| Evaluation Scenario                          | Agent Wins (%) | Avg. Moves Per Game |
|----------------------------------------------|----------------|---------------------|
| Random vs. Random                            | 50.2%          | 83.20               |
| Trained (1000 games) vs. Random              | 55.4%          | 162.75              |
| Trained (2000 games) vs. Random              | 54.8%          | 162.30              |
| Trained (5000 games, Agent First) vs. Random | 56.5%          | 161.03              |
| Trained (5000 games, Random First)           | 55.0%          | 159.89              |
</div>

<br>
- Trained agents extended gameplay significantly, indicating strategic decision-making.
- Performance gains stabilized after extended training, indicating diminishing returns.

---

## Experiment Logging
Training metrics including policy loss, value loss, entropy, and KL divergence were systematically tracked via TensorBoard and Weights & Biases.

---


## Methodology

The project expands upon the baseline PPO algorithm with several enhancements:

### PPO Enhancements:
- **Orthogonal Initialization**: Stabilizes learning through improved gradient flow.
- **Custom Adam Optimizer**: Adjusted epsilon parameter for numerical stability.
- **Generalized Advantage Estimation (GAE)**: Smooths advantage estimates, balancing bias and variance.
- **Mini-Batch Updates**: Improves training stability and reduces catastrophic policy updates.
- **Advantage Normalization**: Keeps the policy updates consistent and numerically stable.
- **Clipped Surrogate Objective**: Prevents large policy deviations, enhancing PPO stability.
- **Value Function Loss Clipping**: Avoids large, destabilizing updates in value predictions.
- **Entropy Bonus**: Encourages sustained exploration throughout training.
- **Global Gradient Clipping**: Protects against exploding gradients.
- **Separate Actor and Critic Networks**: Prevents interference, optimizing performance for complex environments.

---

## Results

### CartPole-v1
The enhanced PPO implementation successfully achieved stable and optimal performance:
- **Episodic Return**: Consistently exceeded 400, demonstrating effective learning and convergence.
- **Entropy Loss**: Decreased gradually, indicating successful exploration-to-exploitation transition.
- **Value and Policy Loss**: Showed steady convergence, validating stable training dynamics.

### Tic-Tac-Toe
Performance improved significantly with training:

<div align="center">

| Checkpoint | Agent Move Order | Wins | Losses | Draws |
|------------|------------------|------|--------|-------|
| Random     | First            | 597  | 268    | 135   |
| Easy       | First            | 680  | 225    | 95    |
| Easy       | Second           | 290  | 636    | 74    |
| Medium     | First            | 775  | 178    | 47    |
| Medium     | Second           | 439  | 543    | 18    |
</div>

- Agent demonstrated increased strategic play when moving first.
- Performance against opponents improved consistently across checkpoints.
- Agent improved but still struggled significantly when moving second.

### Checkers
Notable strategic development was observed:

<div align="center">

| Evaluation Scenario                          | Agent Wins (%) | Avg. Moves Per Game |
|----------------------------------------------|----------------|---------------------|
| Random vs. Random                            | 50.2%          | 83.20               |
| Trained (1000 games) vs. Random              | 55.4%          | 162.75              |
| Trained (2000 games) vs. Random              | 54.8%          | 162.30              |
| Trained (5000 games, Agent First) vs. Random | 56.5%          | 161.03              |
| Trained (5000 games, Random First)           | 55.0%          | 159.89              |
</div>

- Trained agents extended gameplay significantly, indicating strategic decision-making.
- Performance gains stabilized after extended training, indicating diminishing returns.

---

## Experiment Logging
Training metrics including policy loss, value loss, entropy, and KL divergence were systematically tracked via TensorBoard and Weights & Biases, enabling effective debugging and analysis.

---

## Replicating Results
The provided Jupyter Notebook (`Final_Project.ipynb`) contains the code and configurations necessary to replicate all experiments and results. Configurations and hyperparameters used are thoroughly documented within.

---

For detailed analyses, insights, and extended results, please refer to the [Final Project Report](Final_Project_Report.pdf).

