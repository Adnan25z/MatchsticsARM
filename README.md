# Matchsticks Game

This repository contains an ARM assembly implementation of the matchsticks game where a player competes against the computer. The goal is to avoid picking up the last matchstick.

## Features

- Player vs. Computer matchsticks game
- Input validation for player name and matchstick count
- Turn-based gameplay with the computer making random moves
- Graphical representation of matchsticks
- End-of-game win/lose/draw detection and messaging
- Option to play again

## Technologies Used

- ARM Assembly Language
- ARMlite Simulator

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/matchsticks-game.git
    cd matchsticks-game
    ```

2. Load the `.asm` files into the ARMlite simulator.

## Stages of Development

### Stage 1: Game Setup

- Prompts the player to enter their name.
- Prompts the player to enter the number of matchsticks (between 5 and 100).
- Validates inputs and re-prompts if necessary.
- Displays the player's name and the number of matchsticks.

### Stage 2: Single Player Input

- Displays the current player and remaining matchsticks.
- Prompts the player to remove 1-3 matchsticks.
- Validates the player's move.
- Updates and displays the remaining matchsticks.
- Ends the game when no matchsticks remain.

### Stage 3: Human vs. Computer

- Alternates turns between the player and the computer.
- The computer randomly selects 1-3 matchsticks, ensuring it does not exceed the remaining matchsticks.
- Determines the winner based on the matchsticks left.
- Displays appropriate win/lose/draw messages.
- Prompts the player to play again.

### Stage 4: Graphics

- Utilizes ARMlite's graphics display to represent matchsticks.
- Updates the graphical display to reflect the current number of matchsticks after each turn.

## Core Functions

### Game Setup

- **GameSetup**: Initializes game settings, prompts for player name and number of matchsticks.
- **StartNewGame**: Resets the game to initial settings for a new round.

### Game Logic

- **StartGame**: Main game loop where player and computer take turns.
- **PlayerWins**: Displays a message if the player wins.
- **ComputerWins**: Displays a message if the computer wins.
- **Draw**: Displays a message if the game is a draw.

### Input/Output

- **ReadInputStr**: Reads a string input from the player.
- **ReadInputInt**: Reads an integer input from the player.
- **PrintString**: Prints a string to the output.
- **PrintInt**: Prints an integer to the output.

### Utility

- **GenerateRandomNumber**: Generates a random number for the computer's move.
- **display**: Clears and updates the screen with the current matchstick count.
- **EndProgram**: Halts the program.

## Usage

1. Run the assembly code on the ARMlite simulator.
2. Follow the prompts to enter your name and the number of matchsticks.
3. Take turns with the computer to remove 1-3 matchsticks.
4. Try to avoid picking up the last matchstick to win.
5. Choose to play again or end the program.
