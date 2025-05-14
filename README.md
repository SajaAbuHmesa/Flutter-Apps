# 🕹️ Tic-Tac-Toe Game with Timer – Flutter Implementation

This is a **pre-course task for Gaza Sky Geeks** that demonstrates the implementation of a modern Tic-Tac-Toe game using Flutter. The submission includes only the core logic files (`lib/`, `pubspec.yaml`, and `pubspec.lock`) as required.

---
## 📸 Preview 

![image](https://github.com/user-attachments/assets/41c197ae-394f-450d-b434-556d5409128f)

## 📱 Overview

This Flutter application recreates the classic **Tic-Tac-Toe** game with enhancements like:

- Score tracking for both players
- A countdown timer per turn with a circular progress indicator
- Automatic win/draw detection
- Highlighting winning moves
- Responsive and stylish UI

---

## 🎮 Game Features

### Core Gameplay
- Two-player mode (X and O)
- Players alternate turns
- Game ends with a win (3 in a row) or a draw (full board)
- "Play Again" button resets the board

### Enhanced Features
- **Score Tracking:** Persistent across rounds
- **Turn Timer:** 30-second countdown with a circular progress indicator
- **Visual Feedback:** Winning moves are highlighted
- **Responsive UI:** Works well on various screen sizes
- **Custom Styling:** Uses Google Fonts and color theming

---

## 🧱 Code Structure

### Main Components
- `GameScreen` widget: The main interface
- Timer system: Countdown logic and visualization
- Game state management: Tracks turns, board state, and win/draw logic
- UI elements: Scoreboard, grid, timer, buttons

### Key Methods
```dart
startTimer();        // Starts countdown
stopTimer();         // Stops countdown
resetTimer();        // Resets to full 30 seconds
_tapped(index);      // Handles box taps
_checkWinner();      // Detects win or draw
_clearBoard();       // Resets the game
_buildTimer();       // Renders the timer indicator
```

---

## 🔁 State Management

State variables include:
- `displayXO`: Board content
- `matchedIndexes`: Indexes of winning boxes
- `oScore`, `xScore`: Score counters
- `oTurn`: Whose turn it is
- `winnerFound`: Whether the game has ended
- `seconds`: Countdown timer value

---

## ⏱️ Timer Logic

- Implemented using Dart's `Timer.periodic`
- Pauses when the game ends or when time runs out
- Visualized via `CircularProgressIndicator`

---

## 🧠 Win Detection Logic

Checks for 8 win combinations:
- 3 horizontal rows
- 3 vertical columns
- 2 diagonals

Highlights the winning boxes using a custom accent color.

---

## 🛠️ Customization

You can tweak:
- `maxSeconds` for different time limits
- Colors in the `MainColor` class
- Fonts via Google Fonts
- Grid visuals in `GridView.builder`

---

## 📦 Dependencies

```yaml
dependencies:
  flutter:
    sdk: flutter
  google_fonts: ^5.0.0
```

---

## 📂 Note About Repository Content

This repository includes **only the core game files**:

- `lib/` folder (Dart code)
- `pubspec.yaml` and `pubspec.lock` (for package management)

Build folders, platform folders (`android`, `ios`, `web`, etc.), and `.idea/` settings are excluded to keep the repository clean and focused.

---

## 🙌 Acknowledgment

This project is part of the pre-course preparation for the **Gaza Sky Geeks Flutter Bootcamp**.

---





