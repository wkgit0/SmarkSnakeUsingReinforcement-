About:
This project report presents a Snake game AI developed using Q-Learning and the Bellman equation. The AI agent learns optimal strategies by navigating the game environment, collecting food, and avoiding collisions. The Q-Learning algorithm updates action values with the Bellman equation, striking a balance between immediate rewards and future potential gains. The agent's performance evolves through episodes of training, demonstrated by learning curves and gameplay videos. The project showcases the successful application of reinforcement learning to teach an AI agent complex gameplay, exemplifying its potential in diverse problem domains. Future work could involve refining parameters and exploring advanced learning techniques.

Methodology
Environment:
The Snake game environment was designed to provide a grid-based playing area where the snake navigates to eat food. The agent's goal is to maximize its cumulative rewards by learning the optimal path to collect food without colliding with walls or itself.
Q-Learning:
Q-Learning is a model-free reinforcement learning algorithm that learns an optimal policy by iteratively updating action values based on the Bellman equation. The Q-value of a state-action pair is updated 
Exploration-Exploitation:
To balance exploration and exploitation,Initially, the agent explores the environment by taking random actions. As training progresses, the agent gradually shifts towards exploiting its learned knowledge.
Training Process:
The agent underwent a series of training episodes, where it played the Snake game and updated its values. Each episode consisted of multiple steps, with the agent updating values based on the rewards obtained.

Libraries Used
Pygame: A library for creating 2D games and multimedia applications; used for graphics, sound, and user input handling.
Enum: Supports creating enumerations, which are sets of symbolic names for unique values; likely used to define directions for the snake's movement.
Namedtuple: Creates classes with named fields, similar to lightweight data structures. Represent game objects like positions or actions.
Numpy: Offers support for large, multi-dimensional arrays and matrices in Python; potentially used for numerical operations on game states or rewards.
Torch: PyTorch is a deep learning framework used to create and train neural networks for the Snake game AI.
Random: The random module provides functions to generate random numbers, which can be useful for randomizing actions and exploration during training.
Collections.deque: is a data structure used to efficiently store and manage the agent's experiences (game transitions) in a replay memory.
SnakeGameAI: This is presumably a custom class representing the Snake game environment, where the AI agent interacts and learns.
Direction: An enumeration representing possible directions (up, down, left, right) in the Snake game.
Point: A class likely used to represent positions in the Snake game grid.
Linear_QNet: A custom neural network class representing the Q-network architecture used to approximate Q-values.
QTrainer: A custom class for training the Q-learning agent using Q-network updates.

