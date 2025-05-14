# 🕹️ Tic-Tac-Toe Game with Timer – Flutter Implementation

This is a clean Flutter implementation of the classic **Tic-Tac-Toe** game with modern UI and enhanced features, including score tracking, a countdown timer, and win detection with visual feedback.

> ⚠️ **Note:** This repository includes only the `lib/`, `pubspec.yaml`, and `pubspec.lock` files to showcase the core game logic and UI.  
> To run the app, simply create a new Flutter project and replace the default files with those from this repository.

---

## 🎮 Game Features

### Core Gameplay
- Two-player local game (O vs X)
- First player to align 3 marks wins
- Game ends in a draw if all tiles are filled
- Reset the board after each game

### Enhanced Additions
- 🧠 **Score Tracking:** Keeps ongoing scores across rounds
- ⏲️ **Timer System:** 30-second countdown per round with circular visual indicator
- ✨ **Visual Feedback:** Highlights winning moves with custom accent color
- 📱 **Responsive UI:** Adapts to various screen sizes
- 🎨 **Custom Styling:** Google Fonts + a consistent color scheme via `colors.dart`

---

## 📁 Code Structure

### Main Components
- `GameScreen` widget – main game interface
- Game logic and state management
- Countdown timer integration
- UI components: grid, timer, scores, reset button

### Key Methods
- `startTimer()` – starts the round timer
- `stopTimer()` – stops the current timer
- `resetTimer()` – resets the timer to initial state
- `_tapped()` – processes tile taps and switches turns
- `_checkWinner()` – checks for win/draw after each move
- `_clearBoard()` – resets the board for a new round
- `_buildTimer()` – renders the visual timer UI

---

## 🧠 State Management

The app uses local `StatefulWidget` state variables:
- `displayXO` → current board symbols
- `matchedIndexes` → indexes of winning tiles
- `oScore`, `xScore` → persistent player scores
- `oTurn` → boolean to track which player's turn it is
- `winnerFound` → game end state flag
- `seconds` → countdown value for timer

---

## 🏁 Win Detection Logic

Checks 8 possible winning combinations:
- 3 horizontal rows
- 3 vertical columns
- 2 diagonals

If all tiles are filled and no winner, game is a draw.

---

## 🧪 How to Use

1. **Create a new Flutter project**:
   ```bash
   flutter create tic_tac_toe_app
   ```

2. **Replace the following**:
   - Overwrite `/lib` with the one from this repository
   - Replace `pubspec.yaml` and `pubspec.lock` in the root

3. **Get dependencies**:
   ```bash
   flutter pub get
   ```

4. **Run the app**:
   ```bash
   flutter run
   ```

---

## 🔧 Customization

You can easily modify:
- ⏱️ `maxseconds` → to change the round timer
- 🎨 `MainColor` class → update colors
- 🖋️ `customFontWhite` → change fonts
- 📐 `GridView.builder` → adjust layout or tile size

---

## 📦 Dependencies

- [`google_fonts`](https://pub.dev/packages/google_fonts) – for modern font styling

---

## 📸 Preview 

![image](https://github.com/user-attachments/assets/41c197ae-394f-450d-b434-556d5409128f)


