🕹️ Assembly: Endgame
A fun hangman-style word guessing game built with React. Protect the programming world from the tyranny of Assembly by guessing the hidden word before you run out of languages!

📋 Overview
Assembly: Endgame is a small interactive game inspired by hangman. You guess one letter at a time to uncover a mystery programming word.
Each wrong guess “eliminates” a programming language — when you lose all of them, you lose the game!

The project demonstrates:
- State and derived values in React.
- Modular and readable UI logic using reusable maps and conditionals.
- Visual feedback with confetti and dynamic styles via clsx.

🚀 Features
✅ Random word selection for each game.
✅ Colored “language chips” as lives that disappear with wrong guesses.
✅ Farewell messages for each incorrect guess.
✅ Full keyboard interaction — click letters to guess them.
✅ Win animation with confetti 🎉.
✅ Clear accessibility feedback for screen readers.
✅ “New Game” button to reset and play again.

🧩 Tech Stack
React (Vite or CRA) – UI framework
clsx – Conditional class name utility
react-confetti – Confetti celebration on win

🧠 How It Works
The app picks a random word using getRandomWord() at the start.
When a user clicks a letter:
If it’s correct → it appears in the word.
If it’s wrong → a “language chip” disappears.
The player wins when all letters are revealed, or loses when all languages are gone.
When the game ends:
Win → Confetti drops and “You win!” message shows.
Lose → The full word is revealed with a “Game Over!” message.
Custom utilities – getRandomWord and getFarewellText for logic

CSS – For layout and animations
