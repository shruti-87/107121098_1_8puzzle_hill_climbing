# 8-Puzzle Problem using Hill Climbing Variations
This project provides a Python implementation of the 8-puzzle problem using two variations of the hill climbing algorithm:

Random Restart Hill Climbing: Restarts the hill climbing process from a new random configuration when it gets stuck in a local optimum.
First Choice Hill Climbing: Randomly chooses neighbors and selects the first one that improves the current state.
Problem Description
The 8-puzzle is a sliding puzzle that consists of a 3x3 grid of numbered tiles, with one tile missing. The goal is to rearrange the tiles to match a predefined target configuration by moving adjacent tiles into the empty space.

Example:
Initial State:
1  2  5
3  4  
6  7  8

Goal State:
1  4  2
3  5  
6  7  8
The goal is to achieve the goal state from any random initial configuration using heuristic-based algorithms.

##Algorithms
1. Random Restart Hill Climbing:
Starts from a random configuration.
Uses hill climbing to move towards a state with a lower heuristic (Manhattan distance).
Restarts from a new random configuration if stuck in a local optimum, up to a specified number of restarts.
2. First Choice Hill Climbing:
Starts from an initial configuration.
Instead of evaluating all neighbors, randomly checks neighbors and selects the first one that reduces the heuristic.
Stops after a fixed number of failed attempts to improve the state.
Heuristic
The heuristic used in this implementation is the Manhattan Distance, which calculates how far each tile is from its goal position.
