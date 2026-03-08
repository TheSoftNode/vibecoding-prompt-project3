Category: Game

Prompt style: Terse

Title: Color Match Game

Prompt: Color matching game. Display 4 colored boxes: red, blue, green, yellow. Computer randomly picks one color. Player clicks a color to guess. Show "Correct!" in green or "Wrong! It was [color]" in red below the boxes. Add a Reset button labeled "Reset" to play again.

Required libraries: react, tailwindcss

## Rubric

| #   | ID          | Description                                                                                         | Weight | Rationale                                                                                                                                                         | Dependent On |
| --- | ----------- | --------------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render 4 colored boxes for red, blue, green, and yellow                                            | major  | The colored boxes are the main interface elements players interact with.                                                                                          | None         |
| 2   | state       | Pick one color randomly when the game loads                                                        | major  | Random selection creates the challenge by picking which color the player needs to guess.                                                                          | None         |
| 3   | interaction | Check if player clicked the correct color when a box is clicked                                    | major  | This comparison is the core game logic checking if the player guessed correctly.                                                                                  | C1           |
| 4   | interaction | Display "Correct!" or "Wrong! It was [color]" message when player clicks a colored box             | major  | Showing feedback after a click lets the player know if their guess was right or wrong.                                                                            | C3           |
| 5   | interaction | Display "Correct!" message in green and "Wrong!" message in red                                    | minor  | Different colors for success and failure make it faster to see the result without reading.                                                                        | C4           |
| 6   | layout      | Position the feedback messages ("Correct!" or "Wrong! It was [color]") below the colored boxes     | minor  | Placing feedback below the boxes puts it where players naturally look after clicking.                                                                             | C4           |
| 7   | visual      | Display a Reset button                                                                             | major  | The Reset button lets players start a new round.                                                                                                                  | None         |
| 8   | content     | Label the Reset button with the text "Reset"                                                       | minor  | The exact label identifies the button's purpose clearly.                                                                                                          | C7           |
| 9   | interaction | Pick new random color when Reset button is clicked                                                | major  | Resetting picks a new random color so each round is different.                                                                                                    | C7           |

## Justification

The game works exactly as expected with 4 colored boxes for red, blue, green, and yellow. When the game loads, one color gets randomly picked. After clicking a colored box, the correct feedback message appears below the boxes. "Correct!" shows up in green when the right color is clicked, and "Wrong! It was [color]" appears in red showing which color was correct. The Reset button is labeled "Reset" and clicking it starts a new round with a new random color.
