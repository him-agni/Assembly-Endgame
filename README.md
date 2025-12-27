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

## 📚 What I Learned
- **Derived state instead of extra state variables**  
  I learned to compute values like `isGameWon`, `isGameLost`, and `wrongGuessCount` from existing state (`currentWord` and `guessedLetters`) instead of storing everything separately. This keeps the state simpler and reduces bugs.

- **Mapping data to UI elements**  
  I practiced turning arrays (like `languages` and the alphabet string) into visual components using `.map()`, which made the UI more declarative and easier to extend.

- **Conditional styling with `clsx`**  
  I used `clsx` to apply classes like `correct`, `wrong`, `lost`, and `missed-letter` based on the game state, which kept the JSX cleaner than using long inline conditionals.

- **Accessibility with `aria-live` and screen reader text**  
  I added an `aria-live="polite"` region and a visually hidden section to announce game updates (“Correct!”, “Sorry, the letter X…”) so screen reader users can follow along, improving the overall a11y of the app.

- **Component-level feedback and game flow**  
  I learned how to show different UI states (farewell messages, win/lose messages, confetti, and a reset button) based on the same underlying state, instead of creating separate components or pages.

- **Using third-party UI helpers (`react-confetti`)**  
  I integrated a small third-party package to trigger confetti when the player wins, which showed me how to mix UI libraries with my own game logic.



CSS – For layout and animations
