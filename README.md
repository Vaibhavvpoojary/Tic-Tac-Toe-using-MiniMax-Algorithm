# Unbeatable Tic-Tac-Toe Agent (Human vs. AI)

A terminal-based Tic-Tac-Toe game written in Python, featuring an unbeatable AI opponent driven by the **Minimax Algorithm**. The AI evaluates every possible future board state to guarantee it never loses—resulting in either an AI victory or a forced draw.

## 🚀 Features
* **Unbeatable AI:** Powered by a recursive Minimax decision tree engine.
* **Robust Input Validation:** Prevents crashes from invalid characters, out-of-bound numbers, or choosing already-occupied cells.
* **Zero Dependencies:** Runs entirely on standard built-in Python packages.
* **Backtracking State Management:** Modifies and reverts states on a single matrix to optimize memory usage.

## 📋 How It Works: The Minimax Algorithm
The AI agent treats the game as a zero-sum decision tree:
1. **Maximizing Player (AI / 'O'):** Aims to select moves that maximize the final score (+1 for an AI win).
2. **Minimizing Player (Human / 'X'):** Assumed to play perfectly to minimize the AI's score (-1 for a human win).
3. **Terminal States:** Reaching a draw yields a score of `0`.

The recursive function scores every possible branch of the remaining grid layout, filtering upward to pick the optimal mathematical paths on its turn.

## 🛠️ Requirements
* **Python 3.6** or higher.

## 🎮 How to Run

1. Clone or download the script file (e.g., `tictactoe.py`).
2. Open your terminal or command prompt.
3. Execute the script:
   ```bash
   python tictactoe.py
   ```

## 🕹️ Gameplay & Controls
The board positions are mapped to your keyboard's number keys **1 through 9**:

```text
 1 | 2 | 3 
---+---+---
 4 | 5 | 6 
---+---+---
 7 | 8 | 9 
```

* To place your **X** mark, type the number corresponding to an empty cell and press `Enter`.
* Type `exit` at any prompt to quit the application safely.
