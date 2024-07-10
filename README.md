# 2048 Console Game Implementation in C++

## Overview
This project implements the classic 2048 game in a console-based environment using C++. It utilizes a 4x4 array to represent the game board and includes functions for movement, block addition, display, game state checking, and input handling.

## Components

1. **Game Board Representation:**
   - The game board is represented by a 4x4 array `a[4][4]`.

2. **Movement Functions:**
   - `upmove()`, `downmove()`, `leftmove()`, `rightmove()`: Handle tile movements in respective directions, merging identical tiles and shifting non-zero tiles to the appropriate edge.

3. **Block Addition:**
   - `addblock()`: Adds a new tile (2 or 4) to a random empty position after each move.

4. **Display Function:**
   - `disp()`: Displays the current state of the game board.

5. **State Checking:**
   - `check()`: Compares the current board state with the previous state to determine if a move was made.
   - `checkover()`: Checks if the game is over by looking for empty cells or possible merges.

6. **Main Game Loop:**
   - Initializes the board with two tiles (2 and 4).
   - Continuously waits for user input (arrow keys for moves, Esc to quit).
   - Updates the board based on the move and adds a new block if the move was valid.
   - Displays the updated board and checks if the game is over.

7. **Input Handling:**
   - Uses `getch()` (from `conio.h`) to capture arrow key presses:
     - 72: Up, 80: Down, 75: Left, 77: Right, 27: Esc.

8. **Game Over Condition:**
   - The game ends when no more moves are possible.

## Usage
1. Clone the repository:
2. Compile the program:
```bash
g++ -o 2048 2048.cpp
```
3. Run the executable:
```bash
./2048
```
4. Follow the on-screen instructions to play the game using arrow keys for movement and Esc to quit.

