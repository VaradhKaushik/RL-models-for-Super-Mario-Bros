# RL Models for Super Mario Bros

## Project Overview
This project applies Reinforcement Learning (RL) to autonomously play the game Super Mario Bros using the OpenAI Gym environment with the nes-py emulator. Three RL models are evaluated: Deep Q-Networks (DQN), Double Deep Q-Networks (DDQN), and Proximal Policy Optimization (PPO). The primary goal is to assess which model most effectively navigates and masters the game.

## Models and Techniques
### Deep Q-Networks (DQN)
DQN uses a neural network to approximate the optimal action-value function. This method addresses high-dimensional, continuous state spaces by directly estimating the value of each action at a given state.

### Double Deep Q-Networks (DDQN)
DDQN improves upon the standard DQN by reducing overestimations of action values. It utilizes two neural networks: the primary network estimates the action values like in DQN, and the target network provides a stable target for training updates.

### Proximal Policy Optimization (PPO)
PPO, a policy gradient method, optimizes a "proximal" objective function. It enables large updates, efficient data use, and effective policy learning without significant policy divergence, making it ideal for environments like Super Mario Bros.

## Implementation
The models were implemented using Python and the OpenAI Gym API. The nes-py emulator allows interaction with the classic Super Mario Bros game, providing a robust testbed for RL algorithms.

### Environment Setup
- **CPU**: Intel i7-11700
- **GPU**: Nvidia GeForce RTX-3080
- **RAM**: 16GB
- **OS**: Windows 10


## Usage
To run the models, follow these steps:

1. **Navigate to the Submission Directory**:
   ```bash
   cd submission
   ```

2. **Prepare the Environment**:
   Before running the Jupyter notebooks, ensure that all necessary libraries are installed. Uncomment the `pip install` commands in the `.ipynb` files to install the required dependencies.

3. **Run the Jupyter Notebooks**:
   Open the Jupyter notebooks and run the cells to start the training and evaluation of the models:
   ```bash
   jupyter notebook <notebook_name>.ipynb
   ```

Make sure to activate your Python environment or install Jupyter Lab/Notebook if you haven't already, to ensure that you can run the `.ipynb` files.

## Results
Our experiments reveal that DDQN outperforms DQN and PPO in terms of learning efficiency and gameplay success. DDQN not only learns faster but also achieves higher scores on average across multiple runs.

## Future Work
- Explore more complex CNN architectures for DQNs.
- Integrate other RL algorithms like A3C or Rainbow.
- Implement multi-agent learning scenarios.

## Contributions
This project is open for contributions. Whether it's fixing bugs, improving the documentation, or suggesting new features, all contributions are welcome.

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## References
1. Mnih, V., et al. "Human-level control through deep reinforcement learning." Nature 518.7540 (2015): 529.
2. Schulman, J., et al. "Proximal Policy Optimization Algorithms." arXiv preprint arXiv:1707.06347 (2017).
