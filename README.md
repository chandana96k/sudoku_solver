# Sudoku solver using Backtracking

# What is sudoku?
Given a partially filled 9×9 2D array ‘board[9][9]’, the goal is to assign digits (from 1 to 9) to the empty cells so that every row, column, and subgrid of size 3×3 contains exactly one of the digits from 1 to 9. 

# Approach:
Like all other Backtracking problems, Sudoku can be solved by assigning numbers one by one to empty cells. Before assigning a number, check whether it is valid to assign. 

Check that the same number is not present in the current row, current column and current 3X3 subgrid. After checking for validity, assign the number, and recursively check whether this assignment leads to a solution or not. If the assignment doesn’t lead to a solution, then try the next number for the current empty cell. And if none of the number (1 to 9) leads to a solution, return false and print no solution exists.
