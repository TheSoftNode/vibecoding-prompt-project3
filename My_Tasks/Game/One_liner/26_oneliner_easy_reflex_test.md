Category: Game

Prompt style: One_liner

Title: Reflex Tester

Prompt: Red box appears after random delay, click it when turns green, displays reaction time in milliseconds, "Too Early!" if clicked while red.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display box on screen                                | major  | Showing box gives players the target for testing reflexes.                                   | None         |
| 2   | visual      | Show box with red color initially                    | major  | Starting red establishes the waiting state before the reflex test begins.                    | C1           |
| 3   | state       | Wait random delay before color change                | major  | Random delay creates unpredictable timing that tests true reflexes.                          | None         |
| 4   | visual      | Change box color from red to green after delay       | major  | Turning green signals to players that it's time to click and test their reflexes.            | C3           |
| 5   | interaction | Detect box clicks from player                        | major  | Detecting clicks captures the player's reaction attempt.                                     | C1           |
| 6   | state       | Check if box is green when clicked                   | major  | Checking color determines if the player clicked at the right time or too early.              | C5           |
| 7   | state       | Record timestamp when box turns green                | major  | Recording start time enables calculating how fast the player reacted.                        | C4           |
| 8   | state       | Record timestamp when box is clicked                 | major  | Recording click time enables calculating the reaction delay.                                 | C5           |
| 9   | state       | Calculate reaction time in milliseconds              | major  | Calculating difference between green and click times measures reflex speed.                  | C7, C8       |
| 10  | content     | Display reaction time when clicked on green          | major  | Showing milliseconds tells players how fast their reflexes were.                             | C9           |
| 11  | content     | Display "Too Early!" message when clicked on red     | major  | Showing message tells players they clicked before the box turned green.                      | C6           |
| 12  | state       | Reset box to red after displaying result             | major  | Resetting allows players to test their reflexes again with a new random delay.               | C10, C11     |

## Justification

The reflex tester game works as expected for reaction time measurement. A box displays on screen showing red color initially. After a random delay, the box changes color from red to green. When players click the box, the game detects the click and checks if the box is green. The game records timestamps when the box turns green and when it is clicked, then calculates the reaction time in milliseconds by finding the difference. If clicked on green, the reaction time displays showing how fast the player reacted. If clicked while still red, "Too Early!" message displays telling the player they clicked before the signal. After displaying the result, the box resets to red for another reflex test.
