Category: Game

Prompt style: Terse

Title: Number Guessing Game

Prompt: Number guessing game. Computer picks random number 1-100. Player inputs guess and clicks Submit. Show "Too high", "Too low", or "Correct! You won in X guesses" message. Display guess count. Reset button generates a new random number and the guess count automatically resets to zero for the new game.

Required libraries: react, tailwindcss

## Rubric

| #   | ID          | Description                                                               | Weight | Rationale                                                                                                                                 | Dependent On  |
| --- | ----------- | ------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------- |
| 1   | state       | Generate random number between 1 and 100 on game start                    | major  | Generating a random target number establishes the core game objective that the player must discover through their guesses.                 | None          |
| 2   | visual      | Render input field for player guess                                       | major  | The input field is the primary interface element that allows players to enter their numerical guesses.                                     | None          |
| 3   | visual      | Display a Submit button                                                   | major  | The Submit button serves as the trigger for evaluating the player's guess against the target number.                                       | None          |
| 4   | interaction | Compare player guess to target number when Submit is clicked              | major  | This comparison implements the core game logic that determines whether the guess is too high, too low, or correct.                         | C3            |
| 5   | content     | Display "Too high" message when guess exceeds target number               | major  | This feedback message guides the player to adjust their strategy by guessing lower numbers on subsequent attempts.                         | C4            |
| 6   | content     | Display "Too low" message when guess is below target number               | major  | This feedback message guides the player to adjust their strategy by guessing higher numbers on subsequent attempts.                        | C4            |
| 7   | content     | Display "Correct! You won in X guesses" message when guess matches target | major  | This success message confirms the win condition and displays the performance metric showing how many attempts the player needed.           | C4            |
| 8   | content     | Display guess count showing number of attempts made                       | major  | The guess counter provides ongoing performance feedback that helps players track their progress throughout the game.                       | None          |
| 9   | state       | Increment guess count each time Submit is clicked                         | major  | Incrementing the counter on each guess ensures accurate tracking of the player's total attempts for performance measurement.               | C8            |
| 10  | visual      | Display a Reset button                                                    | major  | The Reset button provides the interface control that allows players to start a new game with a fresh target number.                        | None          |
| 11  | interaction | Generate new random number when Reset button is clicked                   | major  | Generating a new random number when resetting ensures each game session has a unique target for the player to discover.                    | C10           |
| 12  | state       | Reset guess count to zero automatically when a new game begins            | major  | Automatically resetting the counter to zero when a new game is detected ensures clean state and accurate attempt tracking without direct user interaction with the counter. | C11           |
