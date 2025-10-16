# 0-1 Multidimensional Multiple Knapsack

## Overview
The task is to solve a 0-1, multidimensional, multiple knapsack problem i.e an item may either be selected or not, must satisfy multidimensional constraints of a knapsack and maximize thenumber of items (weights) across all knapsacks. 

## Proposed solution
The proposed solution makes use of a random mutation hill climbing algorithm starting from empty knapsacks. A tweak is performed by changing the state of a randomly selected item. If the randomly chosen item is not in a knapsack, it is randomly placed into one. If it is already in a knapsack, it is randomly allocated to another one or  removed altogether. The fitness of the new solution is then checked and kept only if it is an improvement. Feasibility of the solutions are checked to ensure that constraints across dimensions are not violated. 

## Setup
To run the program, the following libraries must be correctly installed  
- Icecream
- Numpy
- tqdm
- matplotlib

