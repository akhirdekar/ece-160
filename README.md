# ECE-160: *Programming for Electrical Engineers (C)*

## __The Maze Game__

Created by [Sean Ridel](https://github.com/SeanRidel) and [Abhijeet Khirdekar](https://github.com/akhirdekar)

Welcome to the Maze Game, an implementation of a maze-solving algorithm in C! This program will determine whether a user-inputted maze is solvable. If solvable, the program will trace the quickest path from a given start to a given finish point. 

### Input: 
The user will provide the dimensions of the maze (length and width = rows x columns), a description of the maze's interior using a grid of characters (0 for path space, anything else for wall space), and a start Point (S) and finish points (F) on the exterior walls (row x column).

### Output:
If solvable, the program will output a printed maze with the path traced out (using a dot).
If unsolvable, the program will output a message indicating that the maze is impossible to solve and to enter another maze.

## Execution:
Upon compiling, the program will prompt the user to enter (1) to solve a maze or (2) to generate a random maze.
If the user selects (1), they will then be prompted to enter the maze dimensions.
The maze must be at least 3x3.

Next, the user will be asked to input their own maze. This part can be quite tedious, so we've **attached a separate README.md** file called [**MAZEINPUT.MD**](https://github.com/akhirdekar/ece-160/blob/main/MAZEINPUT.MD) in this repository with premade mazes for you to copy and paste to try out yourself.

Lastly, the solver will prompt you to enter a starting point (S) and a finish point (F). Make sure they are on the exterior of the maze and are in the format "2 1" for row 2, column 1.

If you select (2), you will be prompted to enter the dimensions of a maze and be given an output of two mazes. The second maze is the one you're interested in!

## Constraints:

This program includes two main components: maze solving and maze generation

*Maze Solver:*
  - The exterior walls of the maze must all be 1s.
  - Starting points must be on an exterior wall and have a boundary to enter.

*Maze Generator*
  - The generator only works for square mazes (n x n)
  - The generator will output two mazes, the first being an array of all 1s (n x n) and the second being the random maze that the **user is interested in**
  - The maze generator may generate impossible mazes. The generator tends to generate more solvable mazes with larger parameters (8x8+)

### **Compilation Steps:**
gcc -o maze main.c mazeGenerator.c mazeSolver.c./maze

A [website](https://keesiemeijer.github.io/maze-generator/#generate) that inspired this project.

## Copyright & Licensing

**Copyright (C) 2024 [Sean Ridel](https://github.com/SeanRidel) & [Abhijeet Khirdekar](https://github.com/akhirdekar)**

Distributed under the *MIT License*. See [LICENSE](https://github.com/akhirdekar/ece-160/blob/main/LICENSE) for details.

*This project was created as part of the final project coursework for *ECE-160: Programming for Electrical Engineers*, taught by [Professor Hong](https://github.com/hong3cooper) during the Spring 2024 semester at The Cooper Union.*


