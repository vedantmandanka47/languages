# Problem 8: Snake with Obstacles and Pathfinding

## Part 1 - Problem

Create a grid Snake game with food, static or moving obstacles, growth, score,
wrapping option, and collision rules. Food may appear only in free cells.
Include an automated player using breadth-first search and a safe-tail
strategy; it must avoid paths that trap the snake.

## Part 2 - Input and Output

Input contains dimensions, seed, initial snake, obstacles, wrapping mode, and
directions per tick. Output the grid, score, snake length, and `ALIVE`,
`COLLISION`, or `NO_REACHABLE_FOOD`.

## Part 3 - Constraints, Examples, and Requirements

- A tick is atomic: movement, obstacle updates, food, growth, then collision.
- Food must be reachable when any reachable free cell exists.
- Example: moving into the snake head is legal only when the tail moves away in
  the same tick.
- Test walls, wrapping, self-collision, food exhaustion, and deterministic seeds.
- Implement in Rust and document BFS complexity.
