# Problem 18: Roguelike Deck Builder

## Part 1 - Problem

Implement turn-based deck-building combat with cards, draw and discard piles,
exhaust, energy, block, health, enemy intents, relics, statuses, rewards, and
map choices. Random choices must be seedable and preserved through save/load.

Generate encounters with difficulty constraints and ensure a living player
always has a legal action unless the encounter is complete.

## Part 2 - Input and Output

Input contains a seed, starting deck, map, and commands such as `PLAY card`,
`END_TURN`, `CHOOSE_REWARD`, and `CHOOSE_NODE`. Output hand, energy, health,
enemy intents, events, and the run result.

## Part 3 - Constraints, Examples, and Requirements

- Reject wrong targets, insufficient energy, unavailable cards, and wrong phases.
- Example: an exhausted card cannot return through a discard reshuffle.
- Test reshuffling, exhaustion, status expiration, enemy ordering, and replay.
- The run summary must include damage, turns, cards, and cause of death.
- Implement in Rust and document combat-transition complexity.
