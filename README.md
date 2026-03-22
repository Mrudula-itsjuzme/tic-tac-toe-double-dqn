# Tic-Tac-Toe with Double Deep Q-Networks (Double DQN)

## Overview

This repository features an implementation of the Double Deep Q-Network (Double DQN) reinforcement learning algorithm to master the game of Tic-Tac-Toe.

## Implementation Details

The project utilizes Deep Reinforcement Learning to train an agent that can make optimal moves in a competitive environment. The use of Double DQN helps in reducing the overestimation of Q-values, leading to more stable training.

### Key Features

- **Double DQN Agent**: A neural-network-based agent trained using reinforcement learning.
- **Configurable Environment**: A flexible game environment for training and evaluation.
- **Reproducible Experiments**: Scripts and logs detailing the training progress and agent performance.

## Getting Started

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/Mrudula-itsjuzme/tic-tac-toe-double-dqn.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Training the Agent
Execute the main entry script to begin the training process:
```bash
python main.py
```

## Repository Structure

- **src/**: Core implementation of the Double DQN agent and game logic.
- **docs/**: Architectural notes and research findings.
- **FAI_proj_S3/**: Directory containing project-specific assets and configurations.

## Future Enhancements

- Integration with multi-agent reinforcement learning (MARL).
- Support for larger board sizes and complex game variants.
- Implementation of a user interface for human-versus-AI gameplay.