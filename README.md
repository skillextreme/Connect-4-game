# Connect Four Game in Pygame

This is a simple implementation of the classic Connect Four game using Python and Pygame. The game allows two players to take turns dropping colored discs from the top into a seven-column, six-row vertically suspended grid. The objective is for a player to form a horizontal, vertical, or diagonal line of four of their own discs.

## Prerequisites

Before you can run this game, you need to have Python and Pygame installed on your system.

- **Python**: The game is written in Python, so you need to have Python installed. You can download Python from [python.org](https://www.python.org/downloads/).
- **Pygame**: Pygame is a set of Python modules designed for writing video games. You can install Pygame by running `pip install pygame` in your terminal or command prompt.

## How to Run the Game

1. **Clone the repository** or download the Python script to your local machine.
2. **Open your terminal** or command prompt and navigate to the directory where the game file is saved.
3. **Run the script** by typing `python connect_four.py` and press Enter. Make sure you are using the Python version with Pygame installed.

## Game Features

- **Graphical User Interface**: Utilizes Pygame to render the game board and handle user interactions.
- **Two Player Mode**: Players take turns to play, with one using red discs and the other using yellow discs.
- **Win Detection**: The game automatically detects when a player has won by connecting four discs vertically, horizontally, or diagonally.
- **Restart Option**: Upon the conclusion of a game, players are given the option to restart the game or exit.

## Controls

- **Mouse Click**: Use the mouse to click on the column where you want to drop your disc.
- **Enter Key**: Press Enter to start the game from the start screen.
- **Y/N Keys**: After a game concludes, press Y to restart or N to exit.

## Implementation Details

The game logic is implemented using a combination of Python functions that handle game setup, player moves, win detection, and drawing the game board and pieces. The game state is maintained in a two-dimensional NumPy array, representing the grid where the game is played.

### Key Functions

- `create_board()`: Initializes the game board as a 2D NumPy array filled with zeros.
- `drop_piece()`: Places a player's piece in the selected column.
- `is_valid_location()`: Checks if a move is valid (i.e., if the column selected is not full).
- `get_next_open_row()`: Finds the next open row in the selected column.
- `winning_move()`: Checks for a winning move on the board.
- `draw_board()`: Draws the game board and pieces on the screen.
- `show_start_screen() / restart_game()`: Display the start and restart options to the players.

## Customization

You can customize the game by modifying the constants at the beginning of the script, such as grid size, colors, and window size, to fit your preferences.

