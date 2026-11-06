# Problem 13: Multiplayer Card Draft

## Part 1 - Problem

Create a two-to-eight-player drafting game. Generate seeded packs containing
cards with rarity, cost, tags, effects, and objectives. Players pick one card,
then pass each pack in a configured direction until packs are exhausted.

Add a scoring phase for card combinations and hidden objectives. Serialize and
restore the game without changing the next player or random state.

## Part 2 - Input and Output

Input contains player count, seed, pack configuration, pass direction, and
player picks. Output each pack, legal picks, owned cards, scores, and rankings.

## Part 3 - Constraints, Examples, and Requirements

- A card can belong to only one player and cannot be picked twice.
- Example: picking after a pack has been passed returns `INVALID_ACTION`.
- Test all player counts, rotation direction, pack exhaustion, ties, and restore.
- Deterministic replay must reproduce every pack and ranking.
- Implement in Rust and document round complexity.
