# 🧠 Tic-Tac-Toe Game with AI (Minimax Algorithm)

A terminal-based Tic-Tac-Toe game in Python where you play as **X** and the computer plays as **O** using a simple AI powered by the **Minimax algorithm** and a **heuristic evaluation function**.

---

## 🎯 Objective

Build and demonstrate an intelligent agent (AI) that plays Tic-Tac-Toe optimally using game theory principles. This project showcases:

- AI decision-making with the **Minimax algorithm**
- **Heuristic evaluation** to manage performance with depth-limited search
- Turn-based user interaction with input validation
- Game win/tie detection

---

## 🛠️ Features

- ✅ Fully playable Tic-Tac-Toe game in the terminal
- 🤖 AI opponent using **Minimax with heuristic pruning**
- 🔁 Repeated game loop with state checks
- 🧠 Tracks number of **game states explored**
- ❌ Handles invalid or duplicate moves gracefully
- 🧩 Heuristic favors lines not blocked by the opponent
- 🧪 Depth-limited search to control complexity

---

## 🎮 How to Play

1. Run the script:
   ```bash
   python tictactoe.py
   ```
2. You are **Player X**, and AI is **Player O**
3. A **Reference Board** will show up like this:

   ```
     1 | 2 | 3
   -----------
     4 | 5 | 6
   -----------
     7 | 8 | 9
   ```

4. Enter a number (1-9) to place your X in the corresponding position
5. The AI responds with its move
6. The game continues until either you or the AI wins, or the board is full (tie)

---

## 🧮 Algorithm Explanation

### Minimax with Heuristic

- The **Minimax algorithm** simulates all possible moves up to a certain depth.
- When the depth limit is reached, a **heuristic function** evaluates the board.
- The heuristic gives a score based on how many unblocked lines are available to each player.
- The AI tries to **maximize** its score (O) while the human player tries to **minimize** it (X).

### Heuristic Function

- Adds +1 for every row, column, or diagonal where the opponent hasn’t placed a mark.
- Evaluates board favorability for both players and returns the difference.

---

## 🗂️ Project Structure

```
📁 your-repo/
│
├── tictactoe.py        # Main Python file with game logic and AI
└── README.md           # Game overview and documentation
```

---

## 📦 Requirements

This is a **pure Python** program. No external libraries are required.

- Python 3.x

To run:
```bash
python tictactoe.py
```

---

## 🔍 Example Gameplay

```
Reference Board:
  1 | 2 | 3
-----------
  4 | 5 | 6
-----------
  7 | 8 | 9

Current Board:
    |   |  
-----------
    |   |  
-----------
    |   |  

Enter move (1-9): 5

Current Board:
    |   |  
-----------
    | X |  
-----------
    |   |  

AI plays...

Current Board:
    |   |  
-----------
    | X |  
-----------
  O |   |  
```

---

## 📊 Stats Output

At the end of each game, the program displays:
- The winner or if it’s a tie
- The **number of states explored** by the AI via the `count` variable

Example:
```
Congratulations! You win! 🎉
Number of states explored: 14
```

---

## 💡 Possible Enhancements

- Add **difficulty levels** by adjusting search depth
- Convert to a **GUI** using `tkinter` or `pygame`
- Add **scoreboard** to track multiple rounds
- Optimize heuristic for better AI performance

---

## 📝 License

This project is open-source under the **MIT License**. Feel free to use and modify it for learning or your own projects.

---

## 🙋 Author
**Muqnit Ur Rehman**

Developed as a Python and AI learning exercise. Contributions and suggestions are welcome!

---
```
