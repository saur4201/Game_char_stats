# 🎮 Game Character Stats Tracker

A robust Python command-line utility that tracks and manages game character statistics using foundational Object-Oriented Programming (OOP) architectures. 

## 🛠️ Key Architectural Highlights
* **Data Encapsulation:** Implements strict data hiding using protected attributes (`_health`, `_mana`, `_level`) to prevent accidental internal data leaks or corruption.
* **Input Validation & Guard Rails:** Utilizes customized Python `@property` getter and setter decorators to build hard boundaries (e.g., locking health between 0-100 and mana between 0-50).
* **Cross-Property Dependency Handling:** The `level_up()` method triggers state changes dynamically across multiple property controllers synchronously via their public interfaces.

## 📁 Repository Structure
├── Game_character_stats_Tracker.py  # Core Object-Oriented Class logic
└── README.md             # Project Architectural Documentation

## 🚀 How It Works
```python
# Instantiate a new hero
hero = GameCharacter('Kratos')

# Combat damage simulation is automatically validated and capped by the health setter
hero.health -= 120 
print(hero.health) # Output will gracefully cap at 0 instead of dropping to -20
```
