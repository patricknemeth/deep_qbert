
# Introduction
In this capstone project, I aim to teach an agent to play the classic Atari game Q*bert using reinforcement learning. Specifically, I will explore the Q-learning algorithm and DQN models to learn an optimal policy for navigating the game's environment in order to maximize the AI agent's reward.

Q*bert is a challenging and chaotic game that requires strategic decision-making and rapid adaptation to a fast-paced and dynamic environment.

I first chose the Q-learning algorithm because it is a model-free reinforcement learning method that can learn optimal strategies from accumulated experience and without requiring any prior knowledge of the game's mechanics. 

The significance of this project lies in the broader use of RL techniques to solve complex decision-making problems in real-world appplications such as smart navigation systems or robotics. By successfully training an agent to play Q*bert, I aim to demonstrate the potential of reinforcement learning to learn intricate strategy and adapt to dynamic environments.


# DQN Background
Deep Q-Networks (DQN) extend traditional Q-learning by using deep neural networks to approximate the Q-value function. The key advantages of DQN include:

- Function Approximation: Where traditional Q-learning methods struggle with large state spaces, DQN uses neural networks to approximate the Q-values, which can efficiently handle high-dimensional sensory inputs like raw pixels from video game frames.
- Experience Replay: DQN implements experience replay by storing the agent's experiences at each time step in a replay buffer and then using random samples from this buffer for learning. This approach breaks the similarity of successive learning samples, thus minimizing the risk of catastrophic forgetting and reducing variance in the learning updates.
- Target Network: Stability during learning is enhanced by introducing a separate, slowly updated target network to generate the Q-value targets. This reduces the risk of feedback loops between the Q-values and the target estimates.

# Project Structure
The project is structured into several sections:

- Environment Setup: Initialization of the Q*bert game environment using Gymnasium API.
- Preprocessing: Steps such as image normalization and downsampling to prepare the input for the neural network.
- Network Architecture: Design of the neural network used in the DQN.
- DQN Implementation: Integration of the core DQN components, including the replay buffer, the main and target networks, and the learning algorithm.
- Training: Running the training cycles where the agent interacts with the environment, stores its experiences, and periodically learns from random batches of past experiences.
- Evaluation: Testing the trained model against the game environment to evaluate its performance.
- Potential areas for further research and improvement.
