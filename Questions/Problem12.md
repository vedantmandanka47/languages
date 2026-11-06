# Problem 12: Wordle-Style Solver

## Part 1 - Problem

Implement a Wordle-style game with a dictionary and answer list. For each guess,
return green, yellow, and gray feedback while handling repeated letters
correctly. In hard mode, every known constraint must be used by later guesses.

Add a solver that filters candidates and chooses guesses using expected
information gain or entropy.

## Part 2 - Input and Output

Input contains word length, allowed words, answers, seed, and guesses. Output
feedback for each guess and `SOLVED`, `FAILED`, or `INVALID_GUESS`.

## Part 3 - Constraints, Examples, and Requirements

- Guesses must have the exact length and occur in the allowed dictionary.
- Example: answer `APPLE`, guess `ALLEY` gives feedback `G Y - Y -` using
  remaining letter counts, not one yellow for every matching character.
- Test repeated letters, hard-mode constraints, duplicate dictionary words, and
  candidate counts after each guess.
- Implement in Rust and document filtering/search complexity.
