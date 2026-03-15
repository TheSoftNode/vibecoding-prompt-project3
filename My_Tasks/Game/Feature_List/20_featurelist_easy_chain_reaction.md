Category: Game

Prompt style: Feature_List

Title: Chain Reaction Dots

Prompt: Build a chain reaction clicking game. Display 20 colored dots randomly positioned across the screen. When a user clicks any dot, make it explode with an expanding circle animation. Any dot touched by the expanding circle explodes and creates its own expanding circle, causing a chain reaction. Display a score at the top that adds 1 point for each dot that explodes. After all dots finish exploding, display the final score with a "Play Again" button to reset the game with 20 new random dots.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display 20 colored dots on the screen                    | major  | The dots provide the interactive elements for the chain reaction game.             | None         |
| 2  | layout      | Position dots randomly across the screen                 | major  | Random positioning creates different chain reaction possibilities each game.       | C1           |
| 3  | visual      | Display score at the top                                 | major  | The score shows users how many dots exploded.                                      | None         |
| 4  | interaction | Make dot explode with expanding circle when clicked      | major  | The explosion creates the visual effect and triggers the chain reaction.           | None         |
| 5  | state       | Explode dots touched by expanding circle                 | major  | Chain explosion creates the core gameplay mechanic.                                | C4           |
| 6  | state       | Create expanding circle for each exploded dot            | major  | Each explosion propagating creates the cascading chain reaction effect.            | C5           |
| 7  | interaction | Add 1 point to score for each dot that explodes          | major  | Scoring rewards users for creating larger chain reactions.                         | None         |
| 8  | content     | Display final score after all dots finish exploding      | major  | The final score shows users their total performance.                               | None         |
| 9  | visual      | Display "Play Again" button after explosions finish      | major  | The button lets users restart with a new game.                                     | None         |
| 10 | interaction | Reset game with 20 new random dots when button clicked   | major  | Resetting provides a fresh challenge for another round.                            | None         |

## Justification

The Chain Reaction Dots game works as expected with cascading explosion mechanics. Twenty colored dots display randomly positioned across the screen. A score counter appears at the top. When users click any dot, it explodes with an expanding circle animation. Any dot touched by the expanding circle explodes and creates its own expanding circle, causing a chain reaction. The score adds 1 point for each dot that explodes. After all dots finish exploding, the final score displays with a "Play Again" button that resets the game with 20 new randomly positioned dots.
