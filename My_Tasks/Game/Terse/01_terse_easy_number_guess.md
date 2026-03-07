Category: Game

Prompt style: Terse

Title: Number Guessing Game

Prompt: Number guessing game. Computer picks random number 1-100. Player inputs guess and clicks Submit. Show "Too high", "Too low", or "Correct! You won in X guesses" message below the submit button. Display guess count above the input field. Reset button starts new game with new random number and guess count returns to zero.

Required libraries: react, tailwindcss

## Rubric

| #   | ID          | Description                                                               | Weight | Rationale                                                                                                                                                                   | Dependent On |
| --- | ----------- | ------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | state       | Generate random number between 1 and 100 on game start                    | major  | Generating a random target number establishes the core game objective that the player must discover through their guesses.                                                  | None         |
| 2   | visual      | Render input field for player guess                                       | major  | The input field is the primary interface element that allows players to enter their numerical guesses.                                                                      | None         |
| 3   | visual      | Display a Submit button                                                   | major  | The Submit button serves as the trigger for evaluating the player's guess against the target number.                                                                        | None         |
| 4   | interaction | Compare player guess to target number when Submit is clicked              | major  | This comparison implements the core game logic that determines whether the guess is too high, too low, or correct.                                                          | C3           |
| 5   | content     | Display "Too high", "Too low", or "Correct! You won in X guesses" message based on guess comparison | major  | These feedback messages guide the player by indicating whether their guess was too high, too low, or correct, enabling them to adjust their strategy accordingly. | C4           |
| 6   | content     | Display guess count showing number of attempts made                       | major  | The guess counter provides ongoing performance feedback that helps players track their progress throughout the game.                                                        | None         |
| 7   | layout      | Position the guess count above the input field                            | minor  | Placing the counter above the input field creates a logical visual hierarchy showing progress before interaction.                                                           | C6           |
| 8   | state       | Increment guess count each time Submit is clicked                         | major  | Incrementing the counter on each guess ensures accurate tracking of the player's total attempts for performance measurement.                                                | C6           |
| 9   | visual      | Display a Reset button                                                    | major  | The Reset button provides the interface control that allows players to start a new game with a fresh target number.                                                         | None         |
| 10  | interaction | Generate new random number when Reset button is clicked                   | major  | Generating a new random number when resetting ensures each game session has a unique target for the player to discover.                                                     | C9           |
| 11  | layout      | Position the feedback message below the submit button                     | minor  | Placing the message below the submit button provides clear visual feedback in a consistent location after each guess.                                                       | C5           |
| 12  | state       | Reset guess count to zero when a new game begins                          | major  | Automatically resetting the counter to zero when a new game is detected ensures clean state and accurate attempt tracking without direct user interaction with the counter. | C10          |
