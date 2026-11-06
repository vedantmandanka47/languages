# Problem 11: Card Game Engine

## Part 1 - Problem

Build a reusable blackjack-like engine. Model cards, seeded decks, players,
hands, betting, dealer rules, blackjack, bust, push, split, double down,
insurance, and payouts. The engine must expose phases and reject actions that
are invalid in the current phase.

## Part 2 - Input and Output

Input contains a seed, player bankrolls, bets, and actions such as `HIT`,
`STAND`, `DOUBLE`, `SPLIT`, and `INSURE`. Output cards visible to each player,
phase events, payouts, and final bankrolls.

## Part 3 - Constraints, Examples, and Requirements

- A card cannot be dealt twice until a reshuffle.
- Example: a natural blackjack pays its configured blackjack payout, while a
  21 created after a hit is scored as a normal 21.
- Test ace values, split hands, insurance, bust, push, and insufficient funds.
- Use an injectable seeded random source and complete event log.
- Implement in Rust and document dealing complexity.
