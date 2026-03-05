Category: Game

Prompt style: Terse

Title: Number Guessing Game

Prompt: Number guessing game. Computer picks random number 1-100. Player inputs guess and clicks Submit. Show "Too high", "Too low", or "Correct! You won in X guesses" message. Display guess count. Reset button starts new game.

Required libraries: react, tailwindcss

## Rubric

| ID            | Description                                                                 | Weight | Rationale                                                                      | Dependent On |
| ------------- | --------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| state-1       | Generate random number between 1 and 100 on game start                     | major  | Random number generation establishes the core game objective.                  | None         |
| visual-1      | Render input field for player guess                                         | major  | Input field is the primary interface for guess submission.                     | None         |
| visual-2      | Display a Submit button                                                     | major  | Submit button triggers guess evaluation.                                       | None         |
| interaction-1 | Compare player guess to target number when Submit is clicked                | major  | Comparison logic is the core game mechanic.                                    | visual-2     |
| content-1     | Display "Too high" message when guess exceeds target number                 | major  | High feedback guides player toward correct answer.                             | interaction-1 |
| content-2     | Display "Too low" message when guess is below target number                 | major  | Low feedback guides player toward correct answer.                              | interaction-1 |
| content-3     | Display "Correct! You won in X guesses" message when guess matches target   | major  | Win message confirms success and shows performance metric.                     | interaction-1 |
| content-4     | Display guess count showing number of attempts made                         | major  | Guess counter tracks player performance.                                       | None         |
| state-2       | Increment guess count each time Submit is clicked                           | major  | Counter incrementation requires state update on each guess action.             | content-4     |
| visual-3      | Display a Reset button                                                      | major  | Reset button enables starting a new game.                                      | None         |
| interaction-2 | Generate new random number when Reset button is clicked                     | major  | Reset functionality restarts the game with fresh state.                        | visual-3     |
| state-3       | Reset guess count to zero when Reset button is clicked                      | major  | Counter reset ensures new game starts with clean state.                        | interaction-2 |
