# Minimax Algorithm for Connect4 with a Twist

This repository contains an implementation of the **Minimax algorithm with Alpha-Beta pruning** for the game **Connect4**. The game is enhanced with a unique twist: after each move, there is a 12.5% chance that the board will rotate 90 degrees clockwise, changing the direction of gravity and adding an extra layer of complexity to the game.

The project includes:
- A fully functional Connect4 game with a graphical interface using Pygame.
- An AI opponent powered by the Minimax algorithm with Alpha-Beta pruning.
- A simulation mode to test the AI's performance against a baseline heuristic.


### Key Features

- **Board Rotation**: A 12.5% chance of rotating the board after each move.
- **Gravity Adjustment**: After rotation, pieces fall to the new bottom of the board.
- **Winning Condition**: The winning condition is checked after the rotation and gravity adjustment.

## Algorithms

### Minimax with Alpha-Beta Pruning
The Minimax algorithm is used to determine the best move for the AI player. Alpha-Beta pruning is applied to optimize the search by reducing the number of nodes evaluated in the game tree. The algorithm evaluates possible moves up to a certain depth and selects the move that maximizes the AI's chances of winning while minimizing the player's chances.

### Heuristic Evaluation
The AI uses a heuristic function to evaluate the board state. The heuristic considers:
- The number of consecutive pieces in rows, columns, and diagonals.
- The center column, which is more valuable in Connect4.
- The potential for both the AI and the player to win in the next moves.

## Simulation Mode
The notebook includes a simulation mode where two AI players compete against each other. One AI uses the custom heuristic, while the other uses a baseline heuristic. The simulation runs multiple games to compare the performance of the two heuristics.

