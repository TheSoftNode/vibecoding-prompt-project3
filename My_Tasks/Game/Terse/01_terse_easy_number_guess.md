Category: Game

Prompt style: Terse

Title: Number Guessing Game

Prompt: Number guessing game. Computer picks random number 1-100. Player inputs guess and clicks Submit. Show "Too high", "Too low", or "Correct! You won in X guesses" after each guess. Display guess count. Reset button starts new game with new random number and guess count returns to zero.

Required libraries: react, tailwindcss

## Rubric

| #   | ID          | Description                                                                                         | Weight | Rationale                                                                                                                                                         | Dependent On |
| --- | ----------- | --------------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | state       | Generate random number between 1 and 100 on game start                                              | major  | The game needs a random target number at the start so there's actually something to guess.                                        | None         |
| 2   | visual      | Render input field for player guess                                                                 | major  | You need somewhere to type your guess.                                                            | None         |
| 3   | visual      | Display a Submit button                                                                             | major  | The Submit button is what triggers checking if your guess is right.                                                              | None         |
| 4   | interaction | Compare player guess to target number when Submit is clicked                                        | major  | This comparison is the core game logic - it checks if you guessed too high, too low, or got it right.                                                | C3           |
| 5   | content     | Display "Too high", "Too low", or "Correct! You won in X guesses" message based on guess comparison | major  | The feedback messages tell you how to adjust your next guess or confirm when you've won.                                                              | C4           |
| 6   | state       | Display "Too high" message in red, "Too low" message in blue, and "Correct!" message in green       | major  | Different colors for each message type make it faster to see what happened without reading the full text.                                                         | C5           |
| 7   | content     | Display guess count showing number of attempts made                                                 | major  | The counter tracks how many tries you've taken so you can see your performance.                                                                                   | None         |
| 8   | layout      | Position the guess count above the input field                                                      | minor  | Putting the count above the input field keeps it visible while you're typing your guess.                                                                          | C7           |
| 9   | visual      | Display a Reset button                                                                              | major  | The Reset button lets you start a fresh game when you want to try again.                                                                                          | None         |
| 10  | interaction | Generate new random number when Reset button is clicked                                             | major  | Resetting picks a new random number so each game is different.                                                                                                    | C9           |
| 11  | layout      | Position the feedback message below the submit button                                               | minor  | Placing feedback below the submit button puts it right where you look after clicking.                                                                             | C5           |
| 12  | interaction | Reset guess count to zero when Reset button is clicked                                              | major  | The counter needs to reset when starting a new game so it tracks only the current game attempts.                                                                  | C9           |

## Justification

The game works exactly as expected with an input field for entering guesses and a Submit button. When the Submit button is clicked, the correct feedback message appears after each guess. "Too high" shows up when the guess is above the target, "Too low" appears when it's below, and "Correct! You won in X guesses" displays when you get it right with the actual number shown. The guess count displays and updates properly. When the Reset button is clicked, a new random number gets generated and the guess count returns to zero for the fresh game.
