# Maze Solver

Maze solving project from [Real Python](https://realpython.com).

## Outline

### Part 1

* Use an object-oriented approach to represent the maze in memory
* Visualize the maze and its solution using scalable vector graphics (SVG)

### Part 2

* Create a binary storage format for the mazes
* Solve mazes using `NetworkX`

## Usage

## Requirements & Restrictions

* A given maze is enclosed in a rectangle
* These rectangles are comprised of a grid of square cells
* The cells form passages along straight lines
    * i.e. paths in the maze will only be vertical or horizontal rather than diagonal or circular
* Each cell will be one unit wide
    * important for calculating and comparing the distances later
* Mazes can have only one entrance and one exit
* Mazes can have arbitrary shapes inside the bounding rectangle
    * surround the maze shape with empty squares marked as exterior to form an open space
    * align the maze’s edges with the enclosing rectangle to save some memory
* A few alternative paths can connect them, including paths with cycles that lead back to a place you’ve already visited.
* Solving the maze means finding a path leading from the entrance to the exit
* Each solution should include acyclic paths
    * i.e., a single path location should only be traversed once without backtracking
* Consider only the shortest paths
    * defining the shortest distance is subject to interpretation, as we’ll see in part two.
* In part two, we’ll also introduce enemies and rewards to the maze so that a player can collect extra points and avoid obstacles
