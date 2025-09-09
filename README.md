# Snake Game AI using Deep Q-Learning

This project is an implementation of the classic Snake Game where an AI agent learns to play using **Deep Q-Learning (DQN)**. The game environment is custom-built with **Pygame**, and the AI is trained using **PyTorch**. The agent learns to maximize its score through trial and error, without any hard-coded logic, demonstrating the power of reinforcement learning.

---

### **Key Features**

* **Custom Pygame Environment:** A fully self-made Snake game environment.
* **Deep Q-Network (DQN):** A robust implementation of a DQN using PyTorch.
* **Reinforcement Learning:** The AI learns through an **epsilon-greedy strategy** to balance exploration and exploitation.
* **Dynamic Plotting:** The training process includes a real-time plot of scores and average scores over episodes.

---

### **Reinforcement Learning Setup**

#### **State Space**
The state is represented by an 11-dimensional vector that provides the AI with essential information about the game environment:
* **Danger:** Whether there is an immediate danger (wall or body) to the straight, right, or left of the snake's head.
* **Current Direction:** A one-hot encoded vector indicating the snake's current direction (up, down, left, right).
* **Food Location:** A one-hot encoded vector indicating the relative location of the food (up, down, left, right).

#### **Action Space**
The AI can choose from three possible actions at each step:
* `[Straight, Right, Left]`

#### **Reward Function**
The agent is guided by a simple reward structure:
* **+10:** For eating food.
* **-10:** For a collision or game over.
* **0:** For a regular move.

---

### **Training Progress**

Over time, the agent's performance improves, with its scores increasing and collisions becoming less frequent. The training curve plots both the game score and average score over episodes, providing a clear visual representation of the learning process.

![Training Progress Plot](https://raw.githubusercontent.com/amulya-jayanti/Snake-game/main/SnakeGameAI-video.mov)

---

### **Dependencies**

This project requires the following libraries:
* `pygame`
* `numpy`
* `torch`
* `matplotlib`

---

### **Inspiration**

This project was inspired by Sentdex's tutorial on Snake AI. It includes several custom improvements:

* A modified neural network structure.
* A more efficient reward system.
* A self-made Pygame environment for greater control.
* Cleaner action-state management.
