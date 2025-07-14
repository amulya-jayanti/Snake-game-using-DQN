# Snake-game
🐍 Snake Game AI using Deep Q-Learning\
This project is an implementation of the classic Snake Game with an AI agent trained using Deep Q-Learning (DQN) in a custom-built environment created using pygame. The AI learns to play the game by maximizing its score through trial and error — no hard-coded logic, just pure reinforcement learning.

🚀 Features
- Fully self-made Snake game environment using Pygame
- Deep Q-Network (DQN) implementation with PyTorch
- Short-term and long-term memory training
- Epsilon-greedy strategy for exploration vs. exploitation
- Game loop with dynamic plotting of scores

🧠 Reinforcement Learning Setup

State Space (11-dimensional): Danger straight, right, left

Current direction (left, right, up, down)

Relative location of food (left, right, up, down)

Action Space (3 actions): [Straight, Right, Left]

Reward Function:

+10 for eating food

-10 for collision/game over

0 for regular move

Agent: Uses a Deep Q-Network (Q-Learning with a neural network approximator)

🕹️ Game Environment

- Grid-based game built with Pygame
- Snake movement handled based on the agent’s action
- Random food placement avoiding collision with the snake
- Game ends on wall or self-collision

📦 Dependencies: pygame, numpy, torch, matplotlib

📈 Training Progress:

The agent learns over time with increasing scores and fewer collisions. The training curve plots both the game score and average score over episodes.

💡 Inspiration:

Inspired by Sentdex's tutorial on Snake AI with Pygame and PyTorch, with custom improvements including:

Modified neural network structure

More efficient reward structure

Self-made Pygame environment

Cleaner action-state management
