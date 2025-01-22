# Hangman

## Overview
This is an interactive command-line **Hangman** game built in Bash. It supports multiple players, difficulty levels, and features like hints, scoring, and a high-score system.

## Features
- Difficulty levels: Easy, Medium, Hard.
- Persistent user data with detailed statistics.
- High score tracking.
- Timer option to track performance.
- Hints for players during the game.
- Dynamic Hangman drawing based on incorrect guesses.

---

## Requirements
- **bash**: The script is designed to run on Unix-based systems with Bash installed.
- **wordlist.txt**: A wordlist file located at `./data/wordlist.txt`.

---

## Setup
1. Clone or download the repository.
2. Ensure the following directory structure exists:
    ./data/  
      wordlist.txt  
      hangman_user_data.txt  
      high_score.txt  
3. Populate `wordlist.txt` with words, one per line.

---

## How to Play
1. Run the game script:
    ./hangman_game.sh  
2. Select a player:
    - Continue with an existing player.
    - Create a new player.
3. Choose the difficulty level:
    - Easy (3-5 letters)
    - Medium (6-8 letters)
    - Hard (9+ letters)
4. Guess letters to uncover the hidden word.
5. Win by guessing the word before exhausting your attempts.

---

## Controls
- Input a single letter when prompted to guess.
- Follow the on-screen prompts for navigation (e.g., replay or exit).

---

## Game Mechanics
### Scoring
- **Correct guesses**: +10 points.
- **Incorrect guesses**: -5 points.
- Bonus for guessing the full word.

### Hints
Hints reveal the first and last letters of the word.

### High Score
The script tracks the highest score across all players. If a player beats the high score, it is updated.

### User Statistics
The game saves player data, including:
- Time taken
- Correct and incorrect guesses
- Total score

---

## Example
| Statistic       | Value          |
|------------------|----------------|
| Time taken       | 45s           |
| Correct words    | 3             |
| Wrong words      | 2             |
| Score            | 150           |
| Guesses          | 10            |

---

## Known Issues
- Ensure `wordlist.txt` contains valid words. Missing this file will prevent the game from starting.

---

## License
This project is open-source and free to use. Modify as you wish!
