# 🪨📄✂️ The Syntx RPS Memory Game

---

## 👥 Group Members

| No. | Name | Student ID | Course |
| :-- | :-- | :-- | :-- |
| 1 | Nur Irdina Umairah Binti Ahmad Hafiz | 24005438 | Information Technology |
| 2 | Sashmita A/P Arulthevan | 24007625 | Information Technology |
| 3 | Nurul Aqilah Binti Mat Yusof | 24005791 | Information Technology |
| 4 | Liang Haojia | 25008549 | Information Technology |
| 5 | Nur Fathiah Wajihah Binti Kamaruddin | 24005662 | Information Technology |
| 6 | Muhammad Naeem Aiman Bin Mohd Nasir | 25014188 | Information Technology |
| 7 | Allayar Bekiyev Ahmedovich | 24005516 | Information Technology |
| 8 | Putri Umairul Zahra Binti Mohamad Rafi | 24005826 | Information Technology |

---

## 📖 Project Description

**The Syntx RPS Memory Game** is a C# console-based application that combines the traditional Rock-Paper-Scissors game with a memory challenge.  

Instead of choosing directly, players must memorize a set of cards displayed for a limited time. After the cards are hidden, the computer selects its move, and the player must recall the correct card position that can defeat the computer’s choice.  

This game enhances both logical thinking and memory skills while providing an interactive gameplay experience.

---

## 🎮 System Features

- **Memory-Based Gameplay**  
  Players must memorize card positions before they are hidden.

- **Dynamic Difficulty Levels**

  | Level | Cards | Time Limit | Win Score |
  | :--- | :--- | :--- | :--- |
  | Beginner | 7 | 14 Seconds | 4 Points |
  | Intermediate | 10 | 12 Seconds | 5 Points |
  | Hard | 13 | 10 Seconds | 6 Points |

- **Real-Time Countdown Timer**  
  Smooth countdown using `System.Threading` and `Console.SetCursorPosition`.

- **Score Tracking System**  
  Tracks player progress and determines win conditions.

- **Computer AI Opponent**  
  Generates random moves to simulate gameplay.

- **Robust Input Handling**  
  Uses `try-catch` blocks to prevent crashes from invalid inputs.

---

## 🛠️ OOP Concepts Used

### 🔒 Encapsulation
Encapsulation is implemented by restricting direct access to class data using private and protected fields. Data is accessed through public methods and properties, ensuring controlled interaction and preventing unintended modification.

---

### 🧬 Inheritance
Inheritance is applied through the `Player` class hierarchy. A base `Player` class stores shared attributes such as name and score. The `HumanPlayer` and `ComputerPlayer` classes inherit from it and extend its functionality, reducing code duplication and improving maintainability.

---

### 🔄 Polymorphism
Polymorphism is achieved by defining a common method (`MakeMove()`) in the base `Player` class and allowing each subclass to implement it differently.

- `HumanPlayer` handles user input  
- `ComputerPlayer` generates moves automatically  

This allows the system to treat all players uniformly while maintaining different behaviors.

---

### 🧩 Abstraction
Abstraction is used by hiding complex implementation details and exposing only essential functionalities. For example, the `Player` class defines general behaviors, while the internal logic is handled within its subclasses.

---

## 🚀 Conclusion

The Syntx RPS Memory Game demonstrates the effective use of Object-Oriented Programming concepts to create a modular, scalable, and interactive system. By combining memory challenges with classic gameplay, the project delivers both educational value and entertainment.
* **Power-ups:** Adding special cards that reveal hints or freeze the timer.
* **Multiplayer Mode:** Allowing two players to compete in a memory-off.

---

## 👤 Author
Syntx
