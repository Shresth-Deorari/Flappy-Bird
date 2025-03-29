# Flappy Bird AI - Deep Q-Learning (DQN)

A reinforcement learning-based AI that learns to play Flappy Bird using Deep Q-Networks (DQN). The model is trained using experience replay and reward-based learning to optimize gameplay.

## Features

* **Deep Q-Learning (DQN):** Uses a neural network to approximate Q-values
* **Experience Replay:** Improves learning by storing past experiences
* **Pygame-based Simulation:** Real-time training and testing environment
* **Training Visualization:** Track the agent's learning progress over time

## Setup & Installation

### Prerequisites

* Python 3.x
* TensorFlow / PyTorch
* Pygame

### Installation

# Clone the repository
```
git clone https://github.com/Shresth-Deorari/Flappy-Bird
```
```
cd Flappy-Bird
```
```
pip install -r requirements.txt
```
```
python train.py
```

### Run Trained Model

```
python play.py
```
## How It Works

1. **State Representation:** The game state is represented using key parameters such as bird position, velocity, and pipe distance.
2. **Action Space:** The agent can either flap or do nothing.
3. **Reward System:**
   * +1 for staying alive
   * -100 for hitting an obstacle
4. **Training Process:** The agent improves decision-making by iterating over thousands of episodes and updating Q-values based on game outcomes.

## Project Structure

Flappy-Bird/
├── train.py          # Main training script
├── play.py           # Run pre-trained model
├── dqn_agent.py      # DQN agent implementation
├── flappy_env.py     # Game environment
├── models/           # Saved model checkpoints
├── logs/             # Training logs
└── requirements.txt  # Dependencies

## Results & Future Improvements

✅ Achieves high scores without predefined rules

🔜 **Future improvements:**
- Hyperparameter tuning
- Policy gradient methods
- Better state representation
- Multi-agent competition

## Acknowledgements

This project uses the Pygame library for the game environment and is inspired by the original Flappy Bird game created by Dong Nguyen.
