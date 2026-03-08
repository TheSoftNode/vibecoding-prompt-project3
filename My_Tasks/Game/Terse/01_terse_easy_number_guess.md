Category: Game

Prompt style: Terse

Title: Color Match Game

Prompt: Color matching game. Display 4 colored boxes: red, blue, green, yellow. Computer randomly picks one color. Player clicks a color to guess. Show "Correct!" in green or "Wrong! It was [color]" in red. Reset button to play again.

Required libraries: react, tailwindcss

## Rubric

| #   | ID          | Description                                                                                         | Weight | Rationale                                                                                                                                                         | Dependent On |
| --- | ----------- | --------------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render 4 colored boxes for red, blue, green, and yellow                                            | major  | The colored boxes are the main interface elements players interact with.                                                                                          | None         |
| 2   | state       | Randomly pick one color when the game loads                                                        | major  | Random selection creates the challenge by picking which color the player needs to guess.                                                                          | None         |
| 3   | interaction | Check if player clicked the correct color when a box is clicked                                    | major  | This comparison is the core game logic checking if the player guessed correctly.                                                                                  | C1           |
| 4   | content     | Display "Correct!" or "Wrong! It was [color]" message based on player's choice                     | major  | The feedback messages tell the player if they got it right or what the correct answer was.                                                                        | C3           |
| 5   | state       | Display "Correct!" message in green and "Wrong!" message in red                                    | major  | Different colors for success and failure make it faster to see the result without reading.                                                                        | C4           |
| 6   | visual      | Display a Reset button                                                                             | major  | The Reset button lets players start a new round.                                                                                                                  | None         |
| 7   | interaction | Pick new random color when Reset button is clicked                                                | major  | Resetting picks a new random color so each round is different.                                                                                                    | C6           |
| 8   | layout      | Position the Reset button below the colored boxes                                                 | minor  | Placing the button below the boxes keeps it accessible without blocking the game area.                                                                            | C6           |
| 9   | layout      | Position the feedback message above the Reset button                                              | minor  | Placing feedback above the reset button creates a logical flow from game to result to new game.                                                                   | C4           |

## Justification

The game works exactly as expected with 4 colored boxes for red, blue, green, and yellow. When the game loads, one color gets randomly picked. After clicking a colored box, the correct feedback message appears. "Correct!" shows up in green when the right color is clicked, and "Wrong! It was [color]" appears in red showing which color was correct. The Reset button appears below the boxes to start a new round with a new random color.
