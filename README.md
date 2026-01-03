# 🏓 Pong Game

A classic two-player Pong game built with Python and Turtle Graphics, featuring real-time ball physics, collision detection, and live score tracking.

![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

## 📋 Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [How to Play](#how-to-play)
- [Project Structure](#project-structure)
- [Game Mechanics](#game-mechanics)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)
- [Author](#author)

## ✨ Features

- **Two-Player Mode**: Compete against a friend on the same keyboard
- **Real-Time Physics**: Smooth ball movement with accurate collision detection
- **Dynamic Scoring**: Automatic score tracking displayed on screen
- **Modular Architecture**: Clean OOP design with separated concerns
- **Responsive Controls**: Immediate paddle response to player input
- **Progressive Difficulty**: Ball speed increases as rallies continue

## 🎮 Demo

<img width="997" height="788" alt="image" src="https://github.com/user-attachments/assets/68eb3d76-9c1a-473e-bfea-4b86828a0659" />


## 🚀 Installation

### Prerequisites

- Python 3.x installed on your system
- No external dependencies required (uses built-in Turtle graphics)

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/PrathameshBhosale01/Pong-game.git
   ```

2. Navigate to the project directory:
   ```bash
   cd pong-game
   ```

3. Run the game:
   ```bash
   python main.py
   ```

## 🎯 How to Play

### Controls

| Player | Action | Key |
|--------|--------|-----|
| **Right Paddle** | Move Up | `↑` (Up Arrow) |
| **Right Paddle** | Move Down | `↓` (Down Arrow) |
| **Left Paddle** | Move Up | `W` |
| **Left Paddle** | Move Down | `S` |

### Rules

- Each player controls a paddle to hit the ball back and forth
- Score a point when your opponent misses the ball
- First player to reach the target score wins
- Ball speed increases after each successful paddle hit

## 📂 Project Structure

```
pong-game/
│
├── main.py           # Main game loop and initialization
├── ball.py           # Ball class with movement and collision logic
├── paddle1.py        # Paddle class with movement controls
├── scoreboard.py     # Score tracking and display functionality
├── README.md         # Project documentation

```

### File Descriptions

- **main.py**: Initializes the game window, creates game objects, handles the main game loop, and manages keyboard inputs
- **ball.py**: Contains the Ball class with methods for movement, wall collision, paddle collision, and reset functionality
- **paddle1.py**: Defines the Paddle class with positioning and movement methods
- **scoreboard.py**: Manages the Scoreboard class for displaying and updating player scores

## 🧠 Game Mechanics

### Ball Physics
- Continuous movement using x and y velocity components
- Wall bounce: Reverses y-direction when hitting top/bottom walls
- Paddle bounce: Reverses x-direction with slight speed increase
- Reset mechanism: Returns to center after scoring

### Collision Detection
- **Wall Collision**: Checks if ball's y-coordinate exceeds screen boundaries
- **Paddle Collision**: Uses distance calculation and x-coordinate validation
- **Scoring**: Triggers when ball passes paddle's x-position

### Game Loop
```python
# Pseudocode representation
while game_is_on:
    update_screen()
    move_ball()
    check_wall_collision()
    check_paddle_collision()
    check_scoring()
    update_score()
```

## 🛠️ Technologies Used

- **Python 3.x**: Core programming language
- **Turtle Graphics**: Built-in Python library for 2D graphics
- **OOP Principles**: Class-based design for modularity and reusability

## 🔮 Future Enhancements

- [ ] Single-player mode with AI opponent
- [ ] Multiple difficulty levels (Easy, Medium, Hard)
- [ ] Sound effects for collisions and scoring
- [ ] Pause/Resume functionality
- [ ] Customizable ball and paddle colors
- [ ] Win condition (first to X points)
- [ ] Menu system with game settings
- [ ] Migrate to Pygame for enhanced graphics
- [ ] Web version using JavaScript Canvas

## 📄 License

This project is licensed under the MIT License - feel free to use it for learning and personal projects.

## 👤 Author

**Prathamesh Bhosale**

- GitHub: [@yourusername](https://github.com/PrathameshBhosale01)

## 🙏 Acknowledgments

- Inspired by the classic Pong arcade game (1972)
- Built as a learning project to practice Python and OOP concepts
- Thanks to the Python Turtle Graphics library for making game development accessible

---

⭐ If you found this project helpful, please consider giving it a star!

**Enjoy the game! 🎮**
