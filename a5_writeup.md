# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

BFS seemed more efficient than DFS, as it only goes down a row once it has checked to make sure every other option is good. This is useful because instead of going all the way into one possible outcome, it stops as soon as it hits a an error or solution that doesn't actually work. Personally, I would use BFS if I was making something like this again.

2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

Data structures like stack and queue can greatly increase the functionality of alorithms because they allow you to easily search through a variety of options and figure out which ones aren't possible. They can be used for many more programs than just solving sudoku. I don't know much about other data structures but I am sure there are probably other, similar ways to search through things.

3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

The Sudoku Solver can be used for a variety of puzzle type game where you need to get certain objects/numbers in a certain order. In addition to this, things like DFS and BFS can be used to quickly search for things in more categories than just columns and rows. For example, if you wanted to search for a specific species of animal, you would have to search through a variety of categories such as mammal, genus, etc, which depth-first search could easily do.
