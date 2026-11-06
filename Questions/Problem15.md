# Problem 15: Sokoban Solver

## Part 1 - Problem

Parse a Sokoban level containing walls, goals, crates, and the player. Walking
moves through empty floor; pushing moves one crate into an empty destination.
A crate cannot be pulled. The level is solved when every goal contains a crate.

Implement dead-square detection and an A* or IDA* solver using reverse-push
analysis. Return a legal solution with its movement and push counts.

## Part 2 - Input and Output

Input is an ASCII level followed by optional player moves. Output the board
after each move, invalid actions, and either a solution string, `SOLVED`, or
`UNSOLVABLE`.

## Part 3 - Constraints, Examples, and Requirements

- Preserve the board when a move or push is illegal.
- Example: pushing a crate into a non-goal corner marks the state dead.
- Test multiple crates, already solved levels, deadlocks, and unsolvable levels.
- Replay every returned solution and verify that all crates reach goals.
- Implement in Rust and document A* state complexity.
