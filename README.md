# Welcome to Syntx Rock Paper Scissors Memory Game 🪨📄✂️ 

**Syntx Rock Paper Scissors Memory Game** is a C#-based console application that breathes new life into the classic Rock-Paper-Scissors game. Combining the rules of the traditional hand game with the challenge of memory cards, players must rely on their memory skills rather than just luck to beat the computer.

## 🎮 Game Overview
In this version, the computer displays a set of cards Rock, Paper or Scissors for a limited time depending on the difficulty level. Once the cards are flipped, the computer selects its move. To win the round, you must recall the position of the card that counters the computer's choice.

### Key Features:
* **Memory-Based Mechanics:** Cards are visible for a short duration (10-14 seconds) before being hidden.
* **Real-time Scoring:** Accurate tracking of player and computer progress.
* **Console-Optimized UI:** Uses Console.SetCursorPosition and System.Threading to provide a smooth, flicker-free countdown timer.
* **Dynamic Difficulty Scaling:**
    | Level | Cards | Time Limit | Win Score |
    | :--- | :--- | :--- | :--- |
    | **Beginner** | 7 | 14 Seconds | 4 Points |
    | **Intermediate** | 10 | 12 Seconds | 5 Points |
    | **Hard** | 13 | 10 Seconds | 6 Points |
* **Robust Input Handling:** Features try-catch blocks and input parsing to prevent crashes from invalid user entries.

---

## 🛠️ Technical Architecture (OOP)
The system is built on **Object-Oriented Programming** principles to ensure modularity and scalability. Each component has a dedicated responsibility:

| Class | Responsibility | Key Features |
| :--- | :--- | :--- |
| Card | Represents a game unit | Stores type and handles comparison logic. |
| Level | Manages stage parameters | Determines cardCount and timeLimit. |
| GameCoordinator | Controls game state | Tracks currentLevel and match outcomes. |
| Player | Manages user/AI data | Stores names, scores, and handles input. |
| Timer | Enforces constraints | Calculates timeLeft using DateTime. |
| ScoreTracker | Validates win conditions | Checks if scores meet the requirements. |

* Encapsulation: Private fields in classes like Player1, Level and Timer are protected from external interference, using getter methods for data retrieval. These fields are accessed through public properties or methods, ensuring better data security and preventing unintended modifications.
* Inheritance: Implemented through the Player class hierarchy. A base Player class is created to store common attributes such as name and score. The HumanPlayer and ComputerPlayer classes inherit from this base class and extend its functionality, reducing code duplication and improving maintainability.
* Polymorpism: Achieved by defining a common method (e.g., MakeMove()) in the base Player class and allowing derived classes to provide their own implementations. This enables the program to treat all player types uniformly while executing different behaviors for human and computer players.

---

## 🕹️ How to Play
1.  **Select Difficulty:** Choose your challenge level from the main menu.
2.  **Memorize:** Look at the number of cards. You have a few seconds to memorize where the Rock, Paper and Scissors icons are located.
3.  **The Process:** The computer will announce its move like "Computer choose: Rock".
4.  **Recall:** Type the number of the card that beats the computer (e.g., 1 2 3).
5.  **Win?Lose:** Reach the required points for your level to be declared the champion!

---

## 🚀 Future Enhancements
* **GUI Transition:** Moving from a console-based interface to a graphical.
* **Power-ups:** Adding special cards that reveal hints or freeze the timer.
* **Multiplayer Mode:** Allowing two players to compete in a memory-off.

---

## 👤 Author
Syntx
