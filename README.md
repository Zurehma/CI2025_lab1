# 0-1 Multidimensional Multiple Knapsack

## Overview
The task is to solve a 0-1, multidimensional, multiple knapsack problem i.e an item may either be selected or not, must satisfy multidimensional constraints of a knapsack and maximize the value of items across all knapsacks. 

## Proposed solution
The proposed solution makes use of a random mutation hill climbing algorithm starting from empty knapsacks.  
A tweak is performed by changing the state of a randomly selected item:  
- If the chosen item is not in a knapsack, it is randomly placed into one. 
- If the item is already in a knapsack, it is either randomly moved to a different knapsack or removed altogether.   

Each new candidate solution is evaluated. 
- Its fitness (total value of packed items) is calculated.
- It is accepted only if it improves the fitness of the current solution.
- Feasibility checks ensure that all multidimensional constraints for every knapsack are satisfied.

## Setup
To run the program, the following libraries must be correctly installed  
- Icecream
- Numpy
- tqdm
- matplotlib

