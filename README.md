# Treasure Island Game 🏝️

Treasure Island is a **text-based adventure game** written in **Python**. The player progresses through a series of choices to reach the hidden treasure, while incorrect decisions lead to different game-over outcomes. This project was created as a beginner-friendly Python exercise to practice **user input handling**, **conditional logic**, and **nested decision-making** in a fun and interactive way.

---

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Game Story](#-game-story)
- [Gameplay Logic](#-gameplay-logic)
- [Winning Path](#-winning-path)
- [Losing Paths](#-losing-paths)
- [Features](#-features)
- [Python Concepts Used](#-python-concepts-used)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Source Code](#-source-code)
- [How to Run the Game](#-how-to-run-the-game)
- [Sample Gameplay](#-sample-gameplay)
- [Possible Improvements](#-possible-improvements)
- [Learning Outcomes](#-learning-outcomes)
- [Author](#-author)
- [License](#-license)

---

## 📖 Project Overview

**Treasure Island** is a simple console-based adventure game where the player must make the correct sequence of decisions to find a hidden treasure. The game starts at a crossroad and continues through different stages such as the sea and a mysterious island house with three doors.

The entire game is based on **choice-driven progression**:
- If the player chooses the correct option, the story continues.
- If the player chooses the wrong option, the game ends with a specific failure message.

This makes the project a great example of how to use **nested `if-elif-else` statements** in Python to control program flow.

---

## 🏝️ Game Story

The player is welcomed to **Treasure Island** and given a mission: **find the hidden treasure**.

The journey follows these stages:

1. **Crossroad**  
   The player must choose whether to go **left** or **right**.

2. **Sea**  
   If the player chooses the correct path, they reach the sea and must decide whether to **swim** or **wait** for a boat.

3. **Island House**  
   If the player safely reaches the island, they find a house with **three doors**:
   - **Red**
   - **Yellow**
   - **Blue**

Only one door leads to victory.

---

## 🎮 Gameplay Logic

The game uses a sequence of decisions:

### Step 1: Crossroad
- **left** → Continue the game
- **right** → Reach a desert → **Game Over**

### Step 2: Sea
- **wait** → Safely reach the island
- **swim** → Bitten by a shark → **Game Over**

### Step 3: Door Selection
- **yellow** → Find the hidden treasure → **You Win**
- **red** → Burned by fire → **Game Over**
- **blue** → Frost bite → **Game Over**

---

## 🏆 Winning Path

To win the game, the player must choose the following sequence:

```text
left → wait → yellow
```

If the player follows this exact path, they successfully find the treasure and win the game.

---

## ❌ Losing Paths

The game contains several losing conditions:

| Choice | Result |
|--------|--------|
| `right` | Reached a desert → Game Over |
| `swim` | Bitten by a shark → Game Over |
| `red` | Burned in fire → Game Over |
| `blue` | Frost bite → Game Over |

The game also handles invalid choices by printing an error message such as:
- `Invalid choice. Try again!`
- `Invalid direction. Try again!`
- `Invalid door color. Try again!`

---

## 🚀 Features

- **Interactive text-based gameplay**
- **ASCII art welcome screen**
- **Multiple decision points**
- **Different endings based on player choices**
- **Beginner-friendly Python logic**
- **Simple console interface**
- **Easy to understand and modify**

---

## 🧠 Python Concepts Used

This project practices several important Python basics:

### 1. `print()`
Used to display:
- story narration
- game instructions
- success and failure messages
- ASCII art

### 2. `input()`
Used to collect player choices such as:
- left or right
- swim or wait
- red, yellow, or blue

### 3. `if`, `elif`, `else`
Used to check the player’s input and decide what happens next in the game.

### 4. Nested Conditional Statements
The game logic is built using **nested `if-else` blocks**, which means one decision leads to another decision inside it.

### 5. String Comparison
The game compares user input against expected text values such as:
- `"left"`
- `"wait"`
- `"yellow"`

---

## 🛠️ Technologies Used

- **Python 3**
- **PyCharm** (used for writing/running the project, if applicable)
- **GitHub** (for version control and project hosting)

---

## 📂 Project Structure

```bash
Treasure-Island-Game/
│── treasure_island_game_project.py
│── README.md
```

### File Details

#### `treasure_island_game_project.py`
Contains the full source code of the game, including:
- ASCII art display
- welcome messages
- player input handling
- conditional game logic
- winning and losing outcomes

#### `README.md`
Contains:
- project explanation
- gameplay details
- setup instructions
- sample output
- learning purpose and documentation

---

## 💻 Source Code

Add your Python game file in the repository as **`treasure_island_game_project.py`**. This README is designed to accompany that source file and explain the project structure, gameplay, and learning goals.

---

## ▶️ How to Run the Game

### Method 1: Run using Python
Make sure Python 3 is installed on your system.

1. Download or clone this repository.
2. Open the project folder in **PyCharm**, **VS Code**, or terminal.
3. Run the file using:

```bash
python treasure_island_game_project.py
```

---

## 🔽 Clone This Repository

Use the following command to clone the project from GitHub:

```bash
git clone https://github.com/numair-2003/Treasure-Island-Game.git
```

Then move into the project folder:

```bash
cd Treasure-Island-Game
```

Run the file:

```bash
python treasure_island_game_project.py
```

---

## 🖥️ Sample Gameplay

```text
Welcome to Treasure Island.
Your mission is to find the treasure.

You're at a crossroad! Where would you like to go?
Enter "left" or "right": left

You have reached the sea! There is an island in the middle of the sea.
Enter "swim" or "wait" to wait for the boat: wait

You have finally reached the island! There is a hidden treasure behind one of these three doors in a house.
Enter "red", "yellow", "blue" to select a door: yellow

Congratulations!!!! You have found the hidden treasure. You won!
```

---

## 🔄 Possible Improvements

This project works well as a beginner game, but it can be improved further. Some ideas include:
- adding a **restart option** after Game Over
- using **functions** to organize the code better
- adding **loops** so the player can play multiple times without rerunning the program
- improving input validation
- adding more story branches and levels
- keeping score or tracking attempts
- adding sound or a GUI version in the future

Example improvement for cleaner input handling:

```python
choice = input("Enter your choice: ").lower()
```

This would allow the program to accept inputs like:
- `Left`
- `LEFT`
- `left`

without writing multiple comparisons.

---

## 📚 Learning Outcomes

By building this project, a beginner can learn how to:

- take input from the user
- display formatted output
- use conditional statements to control program flow
- create a simple branching story
- organize a basic Python console project
- upload a project to GitHub and document it using a README file

This project is especially useful for students who are just starting with Python and want a small project to practice programming fundamentals.

---

## 👨‍💻 Author

**Numair Fahad**

---

## 📜 License

This project is open-source and intended for **learning and educational purposes**.