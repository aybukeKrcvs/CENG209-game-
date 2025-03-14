# CENG209-cmd based game
# Dede Korkut Adventures

Welcome to **Dede Korkut Adventures**, a text-based adventure game where you explore various rooms, battle enemies, manage your inventory, and save your game progress. This game offers a rich interactive experience with multiple rooms, items, and enemies to interact with.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Game Commands](#game-commands)
- [Saving and Loading the Game](#saving-and-loading-the-game)
- [Contributing](#contributing)

## Introduction

**Dede Korkut Adventures** is a simple text-based adventure game written in C. Players can move through rooms, fight enemies, and manage an inventory of items, all through a command-line interface. The game also supports saving and loading game states, allowing players to resume their adventures at any time.

## Features

- **Room Exploration**: Navigate through a series of rooms, each with unique descriptions and items.
- **Inventory Management**: Pick up, drop, and use items found in the rooms.
- **Combat System**: Engage in battles with enemies, using weapons and health management.
- **Game State Persistence**: Save your progress to a file and load it later.
- **Command-Line Interface**: Interact with the game using simple commands (e.g., `look`, `inventory`, `move`, `attack`).

## Project Structure

- `main.c`: Contains the main game loop and command processing.
- `game.c` & `game.h`: Game logic for room navigation, combat, and inventory management.
- `save_load.c` & `save_load.h`: Functions to save and load the game state.
- `combat.c` & `combat.h`: Logic for combat between the player and enemies.
- `item.c` & `item.h`: Manages items that the player can pick up and use.

## Installation

### Prerequisites

- A C compiler (e.g., GCC).
- A text editor for viewing and modifying the code.

### Steps to Run the Game

1. Clone the repository:

    ```bash
    git clone https://github.com/aybukeKrcvs/CENG209-game-.git
    cd CENG209 game
    ```

2. Compile the code:

    ```bash
    make
    ```

3. Run the game:

    ```bash
    make run
    ```

    ```bash
    make clean
    ```
    
    ```bash
    make create_saves
    ```

## Game Commands

Here are some commands you can use during the game:

- **look**: View the description of the current room.
- **inventory**: View the items in your inventory.
- **status**: Display the player’s current health and strength.
- **map**: Show a map of the game world.
- **move <direction>**: Move to another room (`up`, `down`, `left`, `right`).
- **pickup <item>**: Pick up an item from the current room.
- **drop <item>**: Drop an item from your inventory into the room.
- **use <item>**: Use an item from your inventory.
- **attack <enemy>**: Attack an enemy with a weapon.
- **save <filename>**: Save the current game state to a file.
- **load <filename>**: Load a saved game state from a file.
- **exit**: Exit the game.

## Saving and Loading the Game

To save and load your game progress, you can use the following commands:

- **save <filename>**: Save the game to a file (e.g., `save mygame.dat`).
- **load <filename>**: Load a saved game from a file (e.g., `load mygame.dat`).

### Example:
save mygame.dat Game saved successfully!

load mygame.dat Game loaded successfully!

## Contributing

Contributions are welcome! If you find a bug or want to improve the game, feel free to fork the repository, make changes, and submit a pull request.

### How to Contribute

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Create a new Pull Request.
