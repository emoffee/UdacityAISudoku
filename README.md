# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: Constrain Propagation is a technique used to reduce search space by defining local constriants in the space. In this project, I narrow down to each pre-defined unit and find ALL THE PAIRS of identical two-digits values(stored in twinboxes_in_a_unit variable as a list). Take the following image as an example, '23' is found in the unit of column3 and will be used to eliminate 2&3 each from the rest of boxes in column 3. If more than one pair are found, they will be sorted and the same procedures are applied one by one.
![image](https://d17h27t6h515a5.cloudfront.net/topher/2017/January/5877cc63_naked-twins/naked-twins.png)
Note that, this 'Naked Twins' strategy is applied together with 'Elimination', 'Only Choice' and 'Search' methods in the reduce_puzzle function.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: A diagonal unit is defined as the required diagonal constraints in initial configuration and is added into the unit collection. Then, the added diagonal constraints will be applied and propagated together with other defined constraints as solver iteratively continues to work.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.



##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.

### Lab

This folder includes my efforts of trial & errors.