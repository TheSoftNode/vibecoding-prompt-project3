Category: Game

Prompt style: Terse

Title: Color Match Game

Prompt: Color matching game. Display 4 colored boxes: red, blue, green, yellow. Computer randomly picks one color and shows it highlighted for 1 second. Player clicks the color they think was highlighted. Show "Correct!" in green or "Wrong! It was [color]" in red after each guess. Display score counting correct guesses. Reset button starts new game with score back to zero.

Required libraries: react, tailwindcss

## Rubric

| #   | ID          | Description                                                                                         | Weight | Rationale                                                                                                                                                         | Dependent On |
| --- | ----------- | --------------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render 4 colored boxes for red, blue, green, and yellow                                            | major  | The colored boxes are the main interface elements players interact with.                                                                                          | None         |
| 2   | state       | Randomly pick one color to highlight on game start                                                 | major  | Random selection creates the challenge by picking which color the player needs to remember.                                                                       | None         |
| 3   | visual      | Highlight the randomly selected color for 1 second                                                  | major  | Highlighting shows the player which color to remember.                                                                                                            | C2           |
| 4   | interaction | Check if player clicked the correct color when a box is clicked                                    | major  | This comparison is the core game logic checking if the player remembered correctly.                                                                               | C1           |
| 5   | content     | Display "Correct!" or "Wrong! It was [color]" message based on player's choice                     | major  | The feedback messages tell the player if they got it right or what the correct answer was.                                                                        | C4           |
| 6   | state       | Display "Correct!" message in green and "Wrong!" message in red                                    | major  | Different colors for success and failure make it faster to see the result without reading.                                                                        | C5           |
| 7   | content     | Display score showing number of correct guesses                                                    | major  | The score tracks how many the player got right so they can see their performance.                                                                                 | None         |
| 8   | layout      | Position the score at the top of the game                                                          | minor  | Putting the score at the top keeps it visible throughout gameplay.                                                                                                | C7           |
| 9   | visual      | Display a Reset button                                                                             | major  | The Reset button lets players start a fresh game when they want to try again.                                                                                     | None         |
| 10  | interaction | Pick new random color when Reset button is clicked                                                | major  | Resetting picks a new random color so each round is different.                                                                                                    | C9           |
| 11  | layout      | Position the feedback message below the colored boxes                                              | minor  | Placing feedback below the boxes puts it right where players look after clicking.                                                                                 | C5           |
| 12  | interaction | Reset score to zero when Reset button is clicked                                                  | major  | The score needs to reset when starting a new game so it tracks only the current game performance.                                                                 | C9           |

## Justification

The game works exactly as expected with 4 colored boxes for red, blue, green, and yellow. When the game starts, one color gets randomly highlighted for 1 second showing which color to remember. After clicking a colored box, the correct feedback message appears. "Correct!" shows up in green when the right color is clicked, and "Wrong! It was [color]" appears in red when the wrong color is clicked. The score displays at the top and updates when correct guesses are made. When the Reset button is clicked, a new random color gets picked and the score returns to zero for the fresh game.
