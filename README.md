# Terminal-based Frogger Game

This project is a Frogger-like game implemented in C for Linux terminals. It uses the ncurses library for terminal-based graphics and local sockets for character movement.

## Project Structure

The project is organized into two main folders:

1. `frogger/`: Contains the implementation using multiple processes.
2. `froggerThread/`: Contains the implementation using threads.

Both versions use local sockets to control the frog's movement in the terminal.

## Requirements

- Linux operating system
- GCC compiler
- ncurses library
- libsdl2-dev libsdl2-mixer-dev library

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/AndreaAresu/frogger-game.git
   cd frogger-terminal-game
   ```

2. Install the ncurses library if not already installed:
   ```
   sudo apt-get install libncurses5-dev libncursesw5-dev
   ```

3. install the libsdl2-dev libsdl2-mixer-dev library if not already installed:
   ```
   sudo apt-get install libsdl2-dev libsdl2-mixer-dev
   ```

## Compilation

### Process Version
```
cd frogger
make
```

### Thread Version
```
cd froggerThread
make
```

## Usage

### Process Version
```
cd frogger
./frogger
```

### Thread Version
```
cd froggerThread
./frogger
```

## Game Controls

- Use arrow keys to move the frog:
  - ↑: Move up
  - ↓: Move down
  - ←: Move left
  - →: Move right
- Press 'q' to quit the game

## Implementation Details

Both versions of the game use the ncurses library for rendering the game in the terminal and local sockets for handling frog movement. The main difference lies in the concurrency model:

1. Process Version: Uses multiple processes to handle game logic, rendering, and input.
2. Thread Version: Uses threads for concurrent execution of game components.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

