Category: Game

Prompt style: Feature List

Title: Memory Card Matching Game

Prompt: Build a memory matching game with 8 pairs of cards (16 cards total) arranged in a 4x4 grid. Each card shows a back side initially. Click a card to flip it and reveal a symbol. Click a second card to reveal it. If the two cards match, keep them face up. If they don't match, flip both back after 1 second. Track number of moves (pairs of flips). Display "You won in X moves!" message when all pairs are matched. Include a Restart button to shuffle and reset the game.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| ID            | Description                                                                 | Weight | Rationale                                                                      | Dependent On |
| ------------- | --------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| layout-1      | Display 16 cards arranged in a 4x4 grid                                     | major  | Grid layout organizes cards in structured playing field.                       | None         |
| visual-1      | Display all cards with back side facing up on initial load                  | major  | Hidden cards create the memory challenge.                                      | None         |
| interaction-1 | Flip card to reveal symbol when clicked                                     | major  | Card flip is the primary game interaction.                                     | visual-1     |
| state-1       | Track first selected card in current turn                                   | major  | First card tracking enables pair comparison.                                   | interaction-1 |
| state-2       | Track second selected card in current turn                                  | major  | Second card tracking completes pair for comparison.                            | interaction-1 |
| state-3       | Compare symbols of two flipped cards after second card is selected          | major  | Symbol comparison implements match detection logic.                            | state-1, state-2 |
| visual-2      | Keep both cards face up when symbols match                                  | major  | Matched cards remain visible to show progress.                                 | state-3      |
| state-4       | Flip both cards back after 1 second when symbols do not match               | major  | Timed flip-back creates memory challenge with visual delay.                    | state-3      |
| content-1     | Display move count showing number of pairs of flips made                    | major  | Move counter tracks player efficiency.                                         | None         |
| state-5       | Increment move count each time two cards are flipped                        | major  | Move incrementation counts each complete turn.                                 | content-1    |
| state-6       | Detect when all 8 pairs are matched                                         | major  | Win condition detection requires tracking all matched pairs.                   | visual-2     |
| content-2     | Display "You won in X moves!" message when all pairs are matched            | major  | Win message confirms game completion with performance metric.                  | state-6      |
| visual-3      | Display a Restart button                                                    | major  | Restart button enables new game initiation.                                    | None         |
| interaction-2 | Shuffle cards and reset game state when Restart button is clicked           | major  | Shuffle creates new random card arrangement for replay.                        | visual-3     |
| state-7       | Reset move count to zero when Restart button is clicked                     | major  | Counter reset ensures clean state for new game.                                | interaction-2 |
