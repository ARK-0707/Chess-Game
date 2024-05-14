# Chess Game Project

## Introduction

Chess is a classic strategy board game played between two players. It is a game of skill, intelligence, and foresight, where each player aims to outmaneuver the opponent and ultimately capture the opponent's king. This project is an implementation of a chess game using the Python programming language and the Pygame library.

![Chessboard](assets\outputs\1.png)

## My Approach

In this project, I have taken an object-oriented programming (OOP) approach to develop the chess game. Each piece (pawn, knight, bishop, rook, queen, and king) is represented as a separate class inheriting from the base `Piece` class. The board is represented as a 2D array of squares, where each square can either be empty or contain a piece.

The game logic is implemented in the `Board` class, which handles the movement of pieces, validation of moves, castling, en passant captures, pawn promotion, and check detection. The `Game` class manages the overall game flow, including the user interface, event handling, and rendering the game board and pieces.

## Features

### Different Themes

The game supports multiple themes, allowing users to change the appearance of the board and pieces. The available themes include green, brown, blue, and gray. Users can switch between themes by pressing the 't' key during the game.

#### Green Theme
![Chessboard](assets\outputs\1.png)

#### Brown Theme
![Chessboard](assets\outputs\2.png)

#### Blue Theme
![Chessboard](assets\outputs\3.png)

#### Gray Theme
![Chessboard](assets\outputs\4.png)

### Move Validation

The game implements strict move validation to ensure that only legal moves are allowed. It checks for potential checks and prevents any move that would put the player's king in check.

#### Validation Moves
![Chessboard](assets\outputs\5.png)
![Chessboard](assets\outputs\6.png)

### Castling

The game supports castling moves for both players. If the king and the corresponding rook have not been moved, and the path between them is clear, the player can castle by moving the king two squares towards the rook.

#### Castling Move
![Chessboard](assets\outputs\7.png)

### En Passant Capture

The game correctly handles en passant captures, which allow a pawn to capture an opponent's pawn that has just advanced two squares from its starting position, passing one of the capturing pawn's starting squares.

#### En Passant Move
![Chessboard](assets\outputs\8.png)

### Check Moves

The game detects when a player's king is in check and only allows moves that would remove the king from check.

#### Check Moves
![Chessboard](assets\outputs\9.png)

### Pawn Promotion

When a pawn reaches the opposite side of the board, it is automatically promoted to a queen.

#### Pawn Promotion Move
![Chessboard](assets\outputs\10.png)

## How to Use the Game

1. Make sure you have Python and the Pygame library installed on your system.
2. Navigate to the project directory and run the `main.py` file.
3. The chess board will be displayed on the screen.
4. To move a piece, left-click on the piece you want to move, and then left-click on the desired square to move the piece.
5. Valid moves will be highlighted on the board.
6. Press the 'r' key to reset the game at any time.
7. Press the 't' key to change the game theme.

## Disclaimer

Please note that this project is not a 100% complete implementation of the chess game. There may be some bugs or issues that I have tried to solve but could not resolve at the moment. I will continue working on improving the game and addressing any known issues. If you encounter any problems or have suggestions for improvement, please feel free to reach out or contribute to the project.