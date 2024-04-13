# Conway's Game of Life - Graphical Game

This project is a graphical game inspired by Conway's Game of Life, built using a Java graphics engine. The game simulates the evolution of cells on a grid based on simple rules, resulting in complex patterns and behaviors.

## Installation

To run the graphical game, follow these steps:

1. Clone this repository to your local machine:

```
git clone https://github.com/Puffy12/Game-of-Life-Java-.git
```

2. Navigate to the cloned directory:

```
cd conways-game-of-life
```

3. Compile and run the `Main.java` file:

```
javac Main.java
java Main
```

## How to Play

The game displays a grid of cells, each of which can be in one of two states: alive or dead. The cells evolve over time based on the following rules:

1. Any live cell with fewer than two live neighbors dies, as if by underpopulation.
2. Any live cell with two or three live neighbors lives on to the next generation.
3. Any live cell with more than three live neighbors dies, as if by overpopulation.
4. Any dead cell with exactly three live neighbors becomes a live cell, as if by reproduction.

## Controls

- Use the mouse to interact with the cells:
  - Left-click to toggle the state of a cell (alive or dead).
  - Right-click to clear the grid and reset all cells to the dead state.
- Press the `Space` key to start or stop the simulation.
- Press the `R` key to reset the simulation to its initial state.
- Press the `/` key to print the game board and display additional commands:
  - `D`: Toggle Delay
  - `F`: Toggle Display Frame Rate
  - `ESCAPE`: Exit the program
  - `H`: Pause rendering
  - `SPACE`: Restart rendering
  - `R`: Reset the GoL Board
  - `S`: Save the GoL Board to a file
  - `L`: Load the GoL Board from a file
  - `U`: Update the board given the `countLiveTwoDegreeNeighbors` rule in the `updateNextCellArray` function

## Implementation Details

The game is implemented using Java and a custom graphics engine. The `Main.java` file initializes the graphical renderer and starts the simulation. The game logic is implemented in the `slGoLBoard.java` class, which manages the state of the grid and applies the rules of Conway's Game of Life. The `spot.java` file contains configuration constants and color settings for the game.

## Customization

You can customize the size of the grid and the initial state of the cells by modifying the constructor parameters in the `slGoLBoard.java` class. Additionally, you can experiment with different rules by modifying the `updateNextCellArray()` method in the same class.

