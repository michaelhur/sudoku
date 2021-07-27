# Sudoku Solver in Python

Sudoku Solver using Backtracking and Crook's Algorithm.

## Backtracking

Backtracking method, most known as **Bruteforce method**, solves the puzzle by substituting every single possible combination from left to right, then top to bottom until every cell is filled.

## Crook's Algorithm

Crook's Algorithm on the other hand attempts to solve the puzzle just like how a human would do. 

1. Mark up all the empty cells.

	a) If the mark-up consists of only one number, fill in the cell with the number.

	b) Remove such number from the mark-up of the cells in the same row, column and subgrid.

2. Find preemptive sets.

	a) Whenever a preemptive set is found, cross out the numbers in the preemptive set from the mark-up of the cells in the same row, column or subgrid.

	b) Repeat until you find no more preemtive set or rule of Sudoku is violated.

3. If the sudoku is not solved by then, or rule of sudoku has not been violated, apply backtracking method from here, but only using the numbers the mark-up instead of all the numbers from 1 to 9.

## Reference

[1] J. F. Crook. A Pencil-and-Paper Algorithm for Solving Sudoku Puzzles. Notices of the American Mathematical Society. 2009.
