# DeepRL Flappy Bird: Solving the Game with Reinforcement Learning

## Overview  
This project implements and evaluates **Reinforcement Learning (RL)** algorithms to train an agent to play the *Flappy Bird* game. The focus is on **Deep Q-Learning (DQN)** and its extensions, including Double DQN, Dueling DQN, and Dueling Double DQN. We also experiment with **Proximal Policy Optimization (PPO)** and **Advantage Actor-Critic (A2C)** to analyze their performance in sparse reward environments.

---

## Features  

- **Environment Transformation**: Custom field-of-view (FoV) with compact state representation for the bird and pipe positions.  
- **Deep Q-Learning Variants**: Implementation of advanced DQN techniques:  
  - DQN  
  - Double DQN  
  - Dueling DQN  
  - Dueling Double DQN  
- **Experimental Comparisons**: Analysis of PPO and A2C methods, their challenges, and potential solutions for sparse rewards.  
- **Performance Optimization**: Hyperparameter sweeps for learning rate, batch size, and exploration decay schedules.  


---

## Algorithms Implemented  

### Deep Q-Learning (DQN) and Extensions  
- **DQN**: Standard Deep Q-Learning with experience replay and neural network optimization.  
- **Double DQN**: Reduces overestimation bias by separating action selection and evaluation.  
- **Dueling DQN**: Splits Q-values into state values and advantages for faster convergence.  
- **Dueling Double DQN**: Combines Double DQN with Dueling architecture for improved performance.  

### Other Attempts  
- **Proximal Policy Optimization (PPO)**: Explored for stability but limited by sparse rewards.  
- **Advantage Actor-Critic (A2C)**: Tested for variance reduction but required sensitive hyperparameter tuning.  

---

## Results  

The **Dueling Double DQN** achieved the best performance:  
- **Average Reward**: 25.42  
- **Standard Deviation**: 22.4  

Comparative results:  
- **Baseline Agent**: Average reward of 3.68  
- **Standard DQN**: Average reward of 24.34  

For detailed performance graphs and experimental insights, refer to the [report](report.pdf).
