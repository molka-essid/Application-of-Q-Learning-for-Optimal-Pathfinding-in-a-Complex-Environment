# Application-of-Q-Learning-for-Optimal-Pathfinding-in-a-Complex-Environment

This project explores the implementation of *Q-Learning*, a reinforcement learning technique, to train an agent to find the *optimal path* in a 2D grid environment with different types of terrains.

##  Project Overview
The main objective is to enable an agent to navigate from a *start position* to a *goal position* while minimizing movement costs and avoiding obstacles.  
The environment is represented as a grid containing:
- *Free cells (0)*: normal path
- *Walls (1)*: impassable obstacles
- *Water (2)*: traversable but costly
- *Start (3)* and *Goal (4)*: initial and target positions

The agent learns through trial and error to optimize its path.

##  Features
- *Custom movement cost function* (move_cost) handling orthogonal and diagonal moves.
- *Reward assignment* (get_reward) for goals, water, invalid moves, etc.
- *Q-Learning training loop* (train_q_learning) for iterative learning.
- *Path extraction* (extract_path) to reconstruct and evaluate the learned optimal path.
- Comparative experiments with different *Q-Learning hyperparameters*.

##  Results
The trained agent successfully:
- Finds a valid path to the goal.
- Minimizes traversal costs by avoiding costly terrains.
- Learns optimal strategies under different reward/penalty settings.

Several test cases are provided:
- *Test 1*: Prioritizing speed, tolerant of water.
- *Test 2*: Balanced avoidance of walls and water.
- *Test 3*: Strong aversion to water, walls largely ignored.

A detailed comparative analysis of steps, total cost, and execution time is included in the report.

##  Technologies
- *Python*
- *NumPy*
- *Matplotlib* (for visualization)
