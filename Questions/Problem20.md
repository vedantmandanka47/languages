# Problem 20: Tournament Game Platform

## Part 1 - Problem

Build a reusable platform that runs seeded tournaments for completed games.
Define common player, game, match-result, ranking, and replay interfaces.
Support round-robin and single-elimination brackets with configurable tie-breakers.

Run independent matches concurrently without sharing mutable game state. Enforce
per-move time limits, checkpoint progress, and resume an interrupted tournament.

## Part 2 - Input and Output

Input contains players, game type, seed, bracket format, scoring rules, and
time limits. Output match events, replay files, standings, tie-break values,
and the final champion.

## Part 3 - Constraints, Examples, and Requirements

- Every match must have a unique deterministic seed and reproducible replay.
- Example: in round-robin, each pair plays exactly once unless configured
  otherwise; rankings use points before secondary tie-breakers.
- Test fixtures with known rankings, ties, timeouts, resume checkpoints, and
  replay equivalence.
- Add a text-based Rust implementation before any graphical interface.
- Document concurrency, ranking, and replay complexity.
