# Tic-Tac-Toe Low-Level Design (LLD)

This repository contains a low-level design (LLD) implementation of the classic Tic-Tac-Toe game. 

## Purpose
This project is created strictly for **learning and educational purposes**. It is designed to understand the core concepts of object-oriented analysis and design, solid principles, and behavioral/structural design patterns as applied to a game architecture.

## Inspiration & References
The implementation and design patterns are inspired by the following resources:
* **Source Reference:** [Concept and Coding - Tic-Tac-Toe Board.java](https://gitlab.com/shrayansh8/interviewcodingpractise/-/blob/main/src/main/java/com/conceptandcoding/LowLevelDesign/LLDTicTacToe/Model/Board.java?ref_type=heads)
* **GitLab Repository:** [Interview Coding Practice by Shrayansh](https://gitlab.com/shrayansh8/interviewcodingpractise)

## Project Structure
```
TicTacToe/
├── LLDTicTacToe/
│   ├── Model/
│   │   ├── Board.java          # Game board with grid and piece placement
│   │   ├── Pair.java           # Utility class for row-column pairs
│   │   ├── PieceType.java      # Enum for X and O
│   │   ├── Player.java         # Player with name and playing piece
│   │   ├── PlayingPiece.java   # Base class for game pieces
│   │   ├── PlayingPieceO.java  # O piece
│   │   └── PlayingPieceX.java  # X piece
│   ├── Main.java               # Entry point
│   └── TicTacToeGame.java      # Core game logic and win detection
└── README.md
```

## Prerequisites
- **Java JDK 8+** installed on your system
- `java` and `javac` available in your terminal/command prompt

Verify installation:
```bash
java -version
javac -version
```

## Setup & Run

### 1. Clone the repository
```bash
git clone https://github.com/patelkanak23/TicTacToe.git
cd TicTacToe
```

### 2. Compile
```bash
javac LLDTicTacToe/Model/*.java LLDTicTacToe/*.java
```

### 3. Run
```bash
java LLDTicTacToe.Main
```

## How to Play
- The game is played on a **3×3 board** between two players (Player1 = X, Player2 = O).
- Players take turns entering their move as `row,column` (0-indexed).
- Example input: `0,0` places a piece at the top-left corner.

```
Board positions:
(0,0) | (0,1) | (0,2)
(1,0) | (1,1) | (1,2)
(2,0) | (2,1) | (2,2)
```

- The game announces the winner or declares a tie if the board is full.
