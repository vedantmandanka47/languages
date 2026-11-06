# Problem 5: Reversi with Search

## Part 1 - Problem

Implement Reversi on an 8 x 8 board. A legal move places a disc in an empty
cell and brackets one or more opponent discs in any of eight directions; all
bracketed discs flip. If a player has no move, that player passes. The game ends
when both players pass or the board is full.

Add a computer opponent using iterative-deepening negamax, alpha-beta pruning,
move ordering, and a transposition table.

## Part 2 - Input and Output

Input contains a mode, seed, and moves as coordinates or `PASS`. Output the board
after each move, legal moves, current score, and the final winner or draw.

## Part 3 - Constraints, Examples, and Requirements

- The initial four discs must be placed according to standard Reversi rules.
- The computer must return the best fully completed search before its time limit.
- Example: a move that brackets three discs flips all three, not just one.
- Test corners, forced passes, terminal boards, and exact final scores.
- Implement in Rust and document search complexity.
