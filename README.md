# Chess_game
 

A simple chess game implemented in Python using the Pygame library.
It features a basic AI that calculates the optimal move by peeking DEPTH moves ahead. The AI assesses positions and scores only.

## Introduction

This is a basic implementation of a chess game with a graphical user interface. The game allows two players to make moves on a standard chessboard. Additionally, there is an AI opponent that uses negamax algorithm, alpha beta pruning for move selection.

## Features

- **Graphical User Interface:**
  - The game features a user-friendly graphical interface developed using the Pygame library.

- **Two-player Mode:**
  - Play against a friend in human vs. human gameplay. Enjoy the classic chess experience with two human players.

- **AI Opponent:**
  - Challenge yourself against an AI opponent equipped with the Negamax algorithm and alpha-beta pruning. The AI has options to make valid moves, providing a single-player chess experience.

- **Checkmate, Stalemate, and Legal Moves:**
  - The game checks for conditions such as checkmate, stalemate, and legal moves, ensuring a fair and rule-compliant gameplay experience.

- **Advanced Chess Mechanics:**
  - Supports advanced chess mechanics, including pawn promotion, en passant, and castling for a more strategic and engaging experience.

- **Undo and Reset Board:**
  - Press Z for undo, R for reset

- **Variety of Chess Boards:**
  - Enjoy playing on different chess board colors, adding a personalized touch to your gaming experience.

- **Immersive Sounds and Images:**
  - Enhance your gaming experience with multiple piece move or capture sounds.

## En Pasant

In chess, the en passant rule allows a pawn to capture an opponent's pawn that has moved two squares forward from its starting position. The capturing pawn moves to the square immediately beyond the captured pawn. Here's how it works:

1. **Initial Position:**:

   <img src="https://github.com/MinDutch03/Chess_game/blob/main/assets/initial_pos.png" alt="Chessboard" width="400"/>

2. **Opponent's Move:**

   <img src="https://github.com/MinDutch03/Chess_game/blob/main/assets/opp_move.png" alt="Chessboard" width="400"/>

3. **En Passant Capture:**

    <img src="https://github.com/MinDutch03/Chess_game/blob/main/assets/En_Passant.png" alt="Chessboard" width="400"/>

## Pawn Promotion:

In chess, pawn promotion occurs when a pawn reaches the eighth rank. The pawn can be promoted to any other chess piece (except a king). Here's how it works:

1. **Reach the Eighth Rank**:
    
   <img src="https://github.com/MinDutch03/Chess_game/blob/main/assets/Eighth's_Rank.png" alt="Chessboard" width="400"/>

2. **Select the Promotion Piece**:

   <img src="https://github.com/MinDutch03/Chess_game/blob/main/assets/Select_promo_piece.png" alt="Chessboard" width="400"/>

## How to Play

1. Clone the repository to your local machine.
   
2. Install the required dependencies.
   
   ```bash
   pip install pygame

3. Run the `main.py` script to start the game.

   ```bash
   python chess/main.py

**Using Visual Studio Code:**

- Open Visual Studio Code.
   
- Click on "File" -> "Open Folder" and select the cloned directory.
   
- Open the integrated terminal in Visual Studio Code.

- Run the following command to start the game:

    ```python
    python chess/main.py
    
## Controls

The controls for the chess game are designed to be intuitive and user-friendly.

- **Selecting a Piece:**
  - Click on the chess piece you want to move. The selected piece will be highlighted to indicate that it's ready for a move.
  - If AI is thinking you can click on AI piece to see all possible moves.

- **Moving a Piece:**
  - After selecting a piece, the legal moves for that piece will be highlighted on the chessboard.
  - Click on one of the highlighted squares to move the selected piece to that position.

The game will automatically handle the rules of chess, including legal moves, capturing opponent pieces, pawn promotion, en passant, and castling.

## Installation

1. Clone the repository:
   
   ```bash
   git clone https://github.com/anuragjain-git/chess-bot.git
   
2. Navigate to the project directory:
   
   ```bash
   cd chess
   
3. Install dependencies:
   
   ```bash
   pip install -r requirements.txt
   
4. Run the game:
   
   ```bash
   python chess/main.py

## Settings for AI

### Human vs Human Gameplay:

If you want to play a game where both players are human:

- Open the `main.py` file and modify the following lines:

   ```python
   SET_WHITE_AS_BOT = False
   SET_BLACK_AS_BOT = False

- To flip the board, go to `engine.py` and set:

   ```python
    self.playerWantsToPlayAsBlack = False

### AI Gameplay:

If you want to play a game with the AI:

- Open the `main.py` file and modify the following lines:

   ```python
   SET_WHITE_AS_BOT = False
   SET_BLACK_AS_BOT = True

- To flip the board, go to `engine.py` and set:

   ```python
    self.playerWantsToPlayAsBlack = False

### DEPTH:

The `DEPTH` setting determines how many moves ahead the AI will consider during its search for the best move. A higher depth generally results in a stronger AI, but it also requires more computational resources.

This emphasizes the recommendation to keep the `DEPTH` value at 3 or lower for a balance between AI strength and computational efficiency.

If you want to modify DEPTH:

- Open the `chessAi.py` file and modify the following lines:

  ```python
   DEPTH = 3

### Acknowledgments:

Special thanks to the Pygame library for providing a straightforward and effective means to develop graphical applications in Python. The ease of use and versatility of Pygame greatly contributed to the creation of this chess engine.

### MIT License

Copyright (c) [2024] [Duc Nguyen]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
