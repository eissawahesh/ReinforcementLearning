# Reinforcement Learning (RL) 

This repository contains three exercises focusing on reinforcement learning (RL) using environments such as multi-armed bandits, CartPole, and Breakout. Each exercise guides you through the implementation of various RL algorithms and their application to different tasks.

## Exercise 1: Multi-Armed Bandits and RL Agents
- **Description:** This exercise introduces the multi-armed bandit problem and involves implementing various RL agents to solve it. You will build and analyze agents such as Random, Greedy, $\epsilon$-Greedy, UCB (Upper Confidence Bound), and REINFORCE (a policy-gradient method). The agents are evaluated on a Bernoulli bandit problem to understand their exploration-exploitation trade-offs.
- **Algorithms and Techniques Used:**
  - Random Agent: Selects actions uniformly at random.
  - Greedy Agent: Selects the action with the highest estimated reward.
  - $\epsilon$-Greedy Agent: Balances exploration and exploitation by selecting the best action with probability $1 - \epsilon$ and exploring with probability $\epsilon$.
  - UCB (Upper Confidence Bound): Incorporates uncertainty into action selection to balance exploration and exploitation.
  - REINFORCE (Policy Gradient): Uses a policy-gradient approach to learn optimal policies, implemented with and without a baseline for variance reduction.

## Exercise 2: Model-Based RL and Dyna-Q
- **Description:** This exercise delves into model-based reinforcement learning through the implementation of the Dyna-Q algorithm. You will use an experience replay buffer to simulate transitions in a grid-world environment and perform Q-learning updates based on both real and simulated experiences. This task illustrates the advantages of model-based learning in improving sample efficiency.
- **Algorithms and Techniques Used:**
  - Q-learning: Updates the action-value function using the observed rewards and the maximum future rewards, applied in a grid-world environment.
  - Dyna-Q: Combines Q-learning with experience replay to enhance learning by leveraging both real-world interactions and simulated experiences stored in a replay buffer.

## Exercise 3: CartPole and Breakout
- **Description:** This combined exercise focuses on training agents in two popular environments: CartPole and Breakout. These tasks demonstrate how reinforcement learning algorithms can be applied to control problems and visual-based games.
  - **CartPole:** In this environment, the objective is to train an agent to balance a pole on a moving cart. The agent learns to maximize the time the pole remains balanced through the application of Q-learning.
  - **Breakout:** This task involves training an agent to play the Atari game Breakout using deep reinforcement learning techniques. The agent learns to control the paddle, keeping the ball in play while breaking bricks.
- **Algorithms and Techniques Used:**
  - Q-learning (CartPole): A model-free algorithm that learns an action-value function to maximize the cumulative reward in the CartPole environment.
  - Deep Q-Networks (DQN) (Breakout): Uses convolutional neural networks (CNNs) to approximate Q-values for each action, allowing the agent to make decisions based on raw visual input.
  - Experience Replay (Breakout): Stores the agent's experiences to break the correlation between consecutive actions and stabilize training by replaying past experiences.

These exercises provide a diverse introduction to reinforcement learning, covering essential algorithms like Q-learning, policy gradients, and model-based approaches. The tasks range from simple multi-armed bandits to complex environments like CartPole and Breakout, providing hands-on experience with RL strategies and their real-world applications.
