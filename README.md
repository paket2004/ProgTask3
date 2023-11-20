# Transportation Problem Solver
This project provides a Python implementation of three popular methods for solving transportation problems: North-West Corner Method, Vogel's Approximation Method, and Russell's Approximation Method.
# Problem Statement
Given the supply and demand constraints, along with the costs associated with transporting goods between sources and destinations, the goal is to find the optimal transportation plan that minimizes the total cost.
# Prerequisites
Python 3.x
# Methods
- North-West Corner Method. Algorithm: Start in the top-left corner of the transportation matrix and iteratively allocate the minimum of supply and demand until all cells are filled.
- Vogel's Approximation Method. Algorithm: Calculate penalties for each row and column, select the cell with the highest penalty, and allocate the minimum of supply and demand. Update penalties and repeat until all cells are filled.
- Russell's Approximation Method. Algorithm: Calculate the rows and columns with maximum values. Create a list of priorities based on the difference between costs and maximum values. Prioritize and allocate cells until all cells are filled.
# Usage
## Define the Linear Programming Problem
```
s = [160, 140, 170]
c = [
    [7, 8, 1, 2],
    [4, 5, 9, 8],
    [9, 2, 3, 6],
]
d = [120, 50, 190, 110]
```
Where:
- `c` is the cost when the product is delivered from source A to destination B.
- `s` is the the supply from the source A to destination B.
- `d` is the demand from the source A to destination B.

### How to Run

1. Define the Linear Programming Problem in the `main.py` section of the script, `c`, `s`, and `d`.
2. Run the `main.py`.
