# Conway's Game of Life with Pygame

This repository contains a Python implementation of Conway's Game of Life, a cellular automaton devised by mathematician John Conway. The game simulates the evolution of a grid of cells based on simple rules, allowing fascinating patterns to emerge. This implementation uses the Pygame library and provides an interactive grid for user input and dynamic simulation.


## Overview
Conway's Game of Life operates on a 2D grid of square cells. Each cell is either alive or dead, and the state of the grid evolves in discrete time steps based on the following rules:

    1. Survival: A live cell with 2 or 3 neighbors survives.
    2. Death: A live cell with fewer than 2 or more than 3 neighbors dies (underpopulation or overpopulation).
    3. Birth: A dead cell with exactly 3 neighbors becomes alive.
The simulation in this repository allows users to design initial states, observe emergent patterns, and interact dynamically with the grid.
## Features

- Interactive Grid:
   - Users can toggle cells on/off with mouse clicks.
- Simulation Controls:
   - Start, pause, reset, and generate random patterns dynamically.
- Dynamic Updates:
   - Grid updates based on user-defined intervals.
- Visualization:
   - Alive cells are displayed in yellow, while the grid background is grey.



## Controls

- Mouse:
   - Left-click on a cell to toggle its state between alive and dead.
- Keyboard:
   - SPACE: Start or pause the simulation
   - C: Clear the grid and reset the simulation.
   - G: Generate a random pattern of alive cells.
   
## Installation

1. Clone the Repository:

```bash
 git clone https://github.com/maitry2710/conways-game-of-life.git
 cd conways-game-of-life

```
2. Install Dependencies: Ensure you have Python installed along with the ```pygame``` library. Install ```pygame``` using:

```bash
pip install pygame
```
## Usage

1. Run the Program:

```bash
python main.py
```
2. Interact:
- Use the mouse and keyboard controls to modify the grid and observe patterns evolve.




## How It Works
1. Grid Representation:

- The grid is represented as a set of tuples where each tuple ```(col, row)``` represents an alive cell.
2. Key Functions:

- ```gen(num):``` Generates a random set of live cells.
- ```draw_grid(positions):``` Draws the grid with alive cells and gridlines.
- ```adjust_grid(positions):``` Applies the Game of Life rules to compute the next generation.
- ```get_neighbors(pos):``` Calculates the neighbors of a given cell.
3. Game Loop:

- The ```main()``` function handles user input, updates the simulation state, and renders the grid frame by frame.
## License

This project works under MIT License. See the [MIT LICENSE](https://choosealicense.com/licenses/mit/) file for details

