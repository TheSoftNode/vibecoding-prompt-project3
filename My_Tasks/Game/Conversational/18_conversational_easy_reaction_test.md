Category: Game

Prompt style: Conversational

Title: Reaction Time Tester

Prompt: I need a reaction time game. Show a gray box with text "Wait for green...". After a random delay between 2-5 seconds, change the box to green and update the text to "Click now!". When I click the green box, measure how many milliseconds it took from green appearing to my click, then display my reaction time. Show a "Try Again" button to reset and play another round.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                  | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------------ | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display rectangular box for game area                        | major  | The box is the interactive target that players watch and click for the reaction test.                            | None         |
| 2   | visual      | Display box in gray color during waiting state               | major  | Gray color signals the waiting state before the reaction challenge begins.                                       | None         |
| 3   | content     | Display text "Wait for green..." during waiting state        | major  | This instruction tells players to watch for the color change and not click prematurely.                          | None         |
| 4   | state       | Wait random delay between 2-5 seconds before changing color  | major  | Random delay prevents players from anticipating the exact moment, testing true reaction speed.                   | None         |
| 5   | visual      | Change box to green color after delay                        | major  | Green color is the signal that triggers the player's reaction and starts timing.                                 | None         |
| 6   | content     | Display text "Click now!" when box turns green               | major  | This instruction confirms to players that they should click immediately.                                         | None         |
| 7   | state       | Record timestamp when box turns green                        | major  | Recording the green timestamp is necessary to calculate how long the player took to react.                       | None         |
| 8   | interaction | Record timestamp when green box is clicked                   | major  | Recording the click timestamp completes the time measurement for calculating reaction speed.                     | C5           |
| 9   | state       | Calculate reaction time in milliseconds from green to click  | major  | Calculating the time difference gives players their precise reaction speed measurement.                          | None         |
| 10  | content     | Display reaction time result after click                     | major  | Showing the result lets players know how fast they reacted and compare across attempts.                          | None         |
| 11  | visual      | Display "Try Again" button after result is shown             | major  | The Try Again button lets players reset and test their reaction time multiple times.                             | None         |
| 12  | interaction | Reset game to waiting state when "Try Again" is clicked      | major  | Clicking Try Again restarts the sequence so players can attempt to improve their time.                           | C11          |
| 13  | layout      | Position "Try Again" button below the reaction box           | minor  | Placing the button below separates the reset control from the main game area.                                    | None         |

## Justification

The application achieved a 92.31% pass rate with one specific failure. A rectangular box displays in gray with text "Wait for green..." during the initial waiting state. After a random delay between 2-5 seconds, the box changes to green and the text updates to "Click now!". The game records the timestamp when green appears. When players click the green box, it records the click timestamp, calculates the reaction time in milliseconds, and displays the result. A "Try Again" button appears after the result, and clicking it resets the game back to the gray waiting state for another round. However, the model failed to position the "Try Again" button below the reaction box. Instead, the button appears to the right of the box or integrated into the results display area, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
