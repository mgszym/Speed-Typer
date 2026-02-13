# SpeedTyper

SpeedTyper is a typing game developed in C++ using the SFML library. The game challenges players to type words quickly and accurately while navigating through various game states such as menus, options, and scoreboards. It is designed to improve typing speed and accuracy in an engaging and interactive way.

## Project Description

The game consists of several components:
- **Menu**: The starting point of the game, allowing players to navigate to different sections such as starting a new game, loading a saved game, viewing the scoreboard, or adjusting options.
- **Game**: The core gameplay where players type words as they appear on the screen. The game tracks the player's score, missed words, and elapsed time.
- **Options**: A settings menu where players can adjust the difficulty level, font style, and word size.
- **Scoreboard**: Displays the top scores achieved by players.
- **End Screen**: Appears when the game ends, allowing players to save their score or return to the main menu.

The game supports saving and loading progress, making it possible to resume a session at any time. It also includes in-game shortcuts for quick actions.

## Features

- **Game States**:
    - Menu
    - Game
    - Options
    - Scoreboard
    - End Screen
- **Save and Load**: Save your progress and load previous games.
- **Scoreboard**: Tracks and displays high scores.
- **Customizable Settings**:
    - Difficulty levels: Easy, Medium, Hard.
    - Font styles: Arial, Pixel.
    - Word sizes: 6, 9, 12.
- **Shortcuts**:
    - `Ctrl + S`: Save the game.
    - `Ctrl + P`: Open options during gameplay.
    - `Ctrl + E`: Quit the game immediately.

## File Structure

- `GameEngine.cpp`: Manages the main game loop, event handling, and state transitions.
- `Menu.cpp`: Handles the main menu and navigation.
- `Game.cpp`: Implements the core gameplay logic, including word rendering, collision detection, and scoring.
- `Options.cpp`: Manages the settings menu and user preferences.
- `Scoreboard.cpp`: Displays and updates the high scores.
- `End.cpp`: Handles the end screen and score submission.
- `Utilities.cpp`: Provides helper functions for word generation and collision checks.
- `Assets/`: Contains required assets such as fonts (`prstartk.ttf`, `arial.ttf`) and text files (`Scoreboard.txt`, `SavedGame.txt`, `ListOfWords.txt`).

## How It Works

1. **Menu Navigation**:
    - Start a new game, load a saved game, view the scoreboard, or adjust settings.
2. **Gameplay**:
    - Words appear on the screen and move horizontally. Players must type the words correctly before they reach the end of the screen.
    - The game ends when the player misses 10 words.
3. **Options**:
    - Adjust the difficulty level, font style, and word size to customize the gameplay experience.
4. **Scoreboard**:
    - View the top scores achieved by players.
5. **End Screen**:
    - Save your score or return to the main menu after the game ends.

## Requirements

- **C++ Compiler**: Compatible with C++17 or later.
- **SFML Library**: Required for graphics rendering and input handling.
- **Assets Folder**: Ensure the `Assets` folder contains the necessary files:
    - `prstartk.ttf` (font)
    - `Scoreboard.txt` (scoreboard data)
    - `ListOfWords.txt` (word list)

## License

This project is for educational purposes. No specific license is applied.
