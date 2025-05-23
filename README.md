# Chess Bot Project

A sophisticated C++ chess engine that implements AI gameplay using the alpha-beta pruning algorithm. This project demonstrates advanced chess mechanics and artificial intelligence concepts in a playable format.

## Project Structure

The project is organized into the following directories and files:

```
├── main.cpp           # Main program entry point
├── Header/           # Core game components
│   ├── bot.cpp       # AI bot implementation
│   ├── chess.cpp     # Chess game logic
│   ├── chess.h       # Chess game declarations
│   ├── path_node.cpp # Path finding utilities
│   └── player.cpp    # Player implementation
├── Gameplay/         # Visual demonstrations
│   └── bot_vs_bot.gif # Game demonstration
└── LICENSE           # MIT License
```

## Features

- Complete chess rule implementation including:
  - All standard piece movements
  - Special moves (castling, en passant)
  - Pawn promotion
  - Fifty-move rule
  - Threefold repetition
- AI opponent using alpha-beta pruning algorithm
- Configurable AI difficulty through decision tree depth
- Command-line interface for gameplay
- Player vs AI and AI vs AI modes

## How to Build and Run

1. Ensure you have a C++ compiler installed (supporting C++11 or later)
2. Open a terminal in the project directory
3. Compile the project using:
   ```sh
   g++ Header/*.cpp main.cpp -std=c++11 -o chess
   ```
4. Run the game:
   ```sh
   ./chess
   ```

## Gameplay Instructions

1. The game uses standard algebraic notation for moves
2. To make a move, enter the source square followed by the destination square (e.g., "e2e4")
3. Special moves:
   - Castling: Move the king two squares towards the rook
   - Pawn promotion: Move the pawn to the last rank, promotion is automatic to queen
   - En passant: Available automatically when conditions are met

## Project Components

- `chess.h/cpp`: Core chess engine implementation
- `bot.cpp`: AI implementation using alpha-beta pruning
- `player.cpp`: Human player interface and move validation
- `path_node.cpp`: Utility for move calculation and board traversal

## Demo

<p align="center">
    <img alt="Chess Bot Gameplay" src="Gameplay/bot_vs_bot.gif" width="1000">
</p>

## Author

👤 **Phạm Lê Ngọc Sơn**

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
