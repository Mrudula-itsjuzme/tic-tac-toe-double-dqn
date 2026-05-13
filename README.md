# Tic-Tac-Toe with Double Deep Q-Networks

A reinforcement-learning project that trains a neural-network agent to play Tic-Tac-Toe using Double Deep Q-Networks, or Double DQN.

The project is intentionally built on a small game environment so the reinforcement-learning loop is easier to inspect, debug, and explain.

---

## Project links and evidence

| Item | Link / Note |
|---|---|
| Repository | https://github.com/Mrudula-itsjuzme/tic-tac-toe-double-dqn |
| Paper / reference | Based on the Double DQN reinforcement-learning concept; no project paper attached |
| Demo video | Not uploaded yet |
| Deployment | Not applicable; local training/evaluation project |
| Dataset note | No external dataset required; experiences are generated through the Tic-Tac-Toe environment |
| Result screenshots / plots | Add training curves, reward plots, and win-rate screenshots under `docs/` when finalized |

---

## Problem statement

Standard DQN can overestimate action values because the same network is used to both choose and evaluate actions. Double DQN reduces this overestimation by separating action selection from action evaluation.

This repository applies that idea to Tic-Tac-Toe as a compact environment for studying value-based reinforcement learning.

---

## What this project includes

- Tic-Tac-Toe game environment
- Double DQN training logic
- neural-network value approximation
- experience replay
- epsilon-greedy exploration
- training and evaluation scripts
- project notes and experiment assets

---

## RL pipeline

```text
Game State
   ↓
Agent selects action
   ↓
Environment returns reward + next state
   ↓
Experience stored in replay buffer
   ↓
Mini-batch training
   ↓
Target network update
   ↓
Improved policy
```

---

## Why Double DQN?

Double DQN improves stability by using:

- an **online network** to choose the best next action
- a **target network** to evaluate that action

This reduces overly optimistic Q-value estimates and usually produces more stable learning than vanilla DQN.

---

## Quick start

```bash
git clone https://github.com/Mrudula-itsjuzme/tic-tac-toe-double-dqn.git
cd tic-tac-toe-double-dqn

pip install -r requirements.txt
python main.py
```

---

## Repository structure

```text
tic-tac-toe-double-dqn/
├── src/            # Double DQN agent and game logic
├── docs/           # architecture notes and research findings
├── FAI_proj_S3/    # project-specific assets/configuration
└── README.md
```

---

## Tech stack

- Python
- Reinforcement Learning
- Deep Q-Learning
- Neural networks
- Experience replay

---

## Future improvements

- add a clean human-vs-agent interface
- compare DQN vs Double DQN directly
- add training curves and win-rate plots
- extend to larger board sizes
- experiment with self-play and multi-agent RL

---

## Author

Built by [Pedamallu Sai Mrudula](https://github.com/Mrudula-itsjuzme) as part of an applied AI and reinforcement-learning portfolio.
