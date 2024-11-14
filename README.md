# Chess Game
A simplified chess game built with Python and Pygame. This project includes a basic AI that uses a negamax algorithm to calculate optimal moves up to a specified depth. It supports all standard chess rules, such as checkmate, stalemate, pawn promotion, en passant, and castling. The game offers both human vs. human and human vs. AI modes, with an adjustable depth setting to balance AI difficulty and performance.

## Key features include:

- **Graphical User Interface:**
  - The game features a user-friendly graphical interface developed using the Pygame library.

- **AI Opponent:** 
  - Challenge a CPU player that makes strategic moves within specified depth limits. Increases the depth creates a more challenging AI. 

- **Standard Chess Rules:** 
  - Full support for advanced rules like en passant and castling.

- **Undo and Reset Options:** 
  - Allows you to undo moves or reset the board. (Press Z for undo. Press R for reset.)

- **Immersive Sounds and Images:**
  - Enhance your gaming experience with multiple piece move, capture, check, and checkmate sounds.

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
   SET_WHITE_AS_BOT = True
   SET_BLACK_AS_BOT = False

- To flip the board, go to `engine.py` and set:

   ```python
    self.playerWantsToPlayAsBlack = False

If you want to change the difficulty of the AI, modify the DEPTH:

- Open the `chessAi.py` file and modify the following lines:

  ```python
   DEPTH = 3

## How to run

- Install dependencies:
   
   ```bash
   pip install -r requirements.txt
   
- Run the game:
   
   ```bash
   python main.py

