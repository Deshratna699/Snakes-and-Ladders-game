# Snakes and Ladders Game

## Overview
The Snakes and Ladders game is a classic board game implemented in Python. This project allows for a configurable board size, a customizable number of players, and various snakes and ladders. Players take turns rolling a die and moving their pieces along the board, aiming to reach the end before anyone else.

## Features
- Configurable board size (n x n)
- Customizable number of players (2-4)
- Configurable snakes and ladders with their start and end positions
- Ability to save and load the game state
- Visualization of player movements using Matplotlib and Seaborn
- Proper exception handling for invalid inputs
- Game history recorded in a text file

## Requirements
- Python 3.x
- Matplotlib
- Seaborn
- Pickle (included with Python standard library)

## Setup Instructions
1. **Install Required Libraries**:
   Make sure you have the required libraries installed. You can install Matplotlib and Seaborn using pip:
   ```bash
   pip install matplotlib seaborn
   ```

2. **Clone the Repository**:
   Clone the repository or download the `snakes_and_ladders.py` file to your local machine.

3. **Run the Game**:
   Open your terminal or command prompt, navigate to the directory where the `snakes_and_ladders.py` file is located, and run:
   ```bash
   python snakes_and_ladders.py
   ```

## How to Play
1. **Enter Board Size**: When prompted, enter the size of the board (e.g., `100` for a 10x10 grid).
2. **Enter Number of Players**: Enter the number of players (between `2` and `4`).
3. **Gameplay**: Players will take turns rolling a die. After rolling, the program will:
   - Display the rolled number
   - Update the player's position
   - Check for snakes or ladders and move the player accordingly
   - Announce if a player has won by reaching the end of the board

4. **Game History**: The game will save the history of moves in a file named `game_history.pkl`. You can load this history if you want to resume a previous game.

5. **Visual Output**: After the game ends, the program will generate and display visualizations of player movements using Matplotlib and Seaborn, saving the plots as `player_moves.png` and `player_moves_seaborn.png`.

## Example Interaction
```
Enter the board size (e.g., 100 for a 10x10 board): 100
Enter number of players (2-4): 2

Turn index: 0, Total players: 2
Player 1 rolled a 4
Player 1 is now at position 4

Turn index: 1, Total players: 2
Player 2 rolled a 3
Player 2 is now at position 3

Turn index: 0, Total players: 2
Player 1 rolled a 2
Player 1 is now at position 6
...
```

## Output Files
- **Game History**: The game history is saved in a file named `game_history.pkl`.
- **Player Movement Visuals**: Player movements are visualized and saved in:
  - `player_moves.png`
  - `player_moves_seaborn.png`

## Exception Handling
The game includes exception handling to manage invalid inputs and ensure a smooth experience. If an invalid number of players is entered, the game will raise an error.

## Contributing
Feel free to fork the repository and submit pull requests for any enhancements or bug fixes. 

## License
This project is open-source and available for use and modification.
