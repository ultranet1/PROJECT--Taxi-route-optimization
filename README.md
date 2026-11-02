# Urban Taxi-v3 Reinforcement Learning Agent

An optimal route planning agent built using Gymnasium's `Taxi-v3` environment and Q-Learning to solve urban passenger pickup and drop-off navigation challenges.

## Key Features
* **Environment Setup**: Simulated 5x5 grid environment with 500 discrete states and 6 actions.
* **Q-Learning Algorithm**: Model-free RL using an $\epsilon$-greedy policy ($\alpha=0.1, \gamma=0.99, \epsilon=0.1$).
* **Policy Training**: Trained across 2,000 episodes to maximize rewards and eliminate penalties.
* **Visualization**: Generates animated GIF clips tracking the agent's behavior during test evaluation.

## Environment Details
* **Action Space**: 0: South, 1: North, 2: East, 3: West, 4: Pickup, 5: Drop-off
* **Rewards**: `-1` per step penalty, `+20` for successful passenger delivery, `-10` for illegal pickup/drop-off.

## Installation & Requirements
Run the following commands to install required dependencies:.
```bash
pip install gymnasium imageio
pip install gymnasium[toy-text]