# A3C-implementation-of-Atari-Environment---Kung-Fu-Master

This project demonstrates the implementation of the **Asynchronous Advantage Actor-Critic (A3C)** algorithm to train an agent on the classic Atari game **Kung Fu Master** using Python and Gymnasium. The approach leverages parallelism to stabilize and speed up reinforcement learning.

---


### Major Components:

-  **Environment Setup**: Installs and configures `gymnasium`, Atari environments, and required libraries.
-  **Model Architecture**: Defines the neural network used by both actor and critic agents.
-  **Worker Agents**: Multiple agents running in parallel environments.
-  **Training Loop**: Asynchronous updates to the global network using thread-safe operations.
-  **Logging**: Performance metrics like reward over episodes are tracked for evaluation.

---

## Getting Started

### 🔧 Requirements

Make sure you’re using **Google Colab** or an environment with access to:

- Python ≥ 3.7
- gymnasium[atari]
- numpy
- torch
- matplotlib

---

## 🧠 What is A3C?

**A3C** is a reinforcement learning algorithm where:
- Multiple agents explore different environments in parallel.
- Each agent has a copy of the network and updates the global network asynchronously.
- This increases stability and efficiency over single-threaded approaches like DQN.

---

## 🎮 Environment

- Game: `KungFuMaster-v4`
- Source: [Atari 2600 via Gymnasium](https://gymnasium.farama.org/environments/atari/)

---

## 📊 Results

- The agent learns to defeat enemies in the game by maximizing long-term reward.
- Trained model shows improved game-play performance over episodes.

*(Graphs & logs are available inside the notebook)*


## License

This project is open-source under the [MIT License](LICENSE).


- Want to test your own Atari games? Just swap `KungFuMaster-v0` with any other Gym Atari env.
- Try fine-tuning hyperparameters for better convergence.

---

