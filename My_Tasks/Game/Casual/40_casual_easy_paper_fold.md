Category: Game

Prompt style: Casual

Title: Toast Browning Timer

Prompt: Show white bread slice and target shade above. Click Start to toast bread. Bread browns gradually. Click Stop to freeze. Win when shade matches target.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                    | Weight | Rationale                                                                             | Dependent On |
| --- | ----------- | ---------------------------------------------- | ------ | ------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display white bread slice                      | major  | The white bread slice provides the object that changes color during toasting.         | None         |
| 2   | content     | Display target shade above bread               | major  | The target shade shows players the goal browning level they must achieve to win.      | None         |
| 3   | visual      | Display Start button                           | major  | The Start button gives players control to begin the toasting process.                 | None         |
| 4   | interaction | Begin browning bread when Start clicked        | major  | Clicking Start initiates the gradual color change from white to brown.                | C3           |
| 5   | state       | Gradually brown bread from white to golden     | major  | Gradual browning simulates realistic toasting progression over time.                  | C4           |
| 6   | visual      | Display Stop button                            | major  | The Stop button gives players control to freeze the browning at desired shade.        | None         |
| 7   | interaction | Freeze browning when Stop clicked              | major  | Clicking Stop halts the color change to lock in the current shade.                    | C6           |
| 8   | state       | Detect when bread shade matches target shade   | major  | Detection determines when the player has achieved the win condition.                  | C5           |
| 9   | content     | Display win message when shades match          | major  | The win message communicates victory to the player when the puzzle is solved.         | C8           |

## Justification

The toast browning timer game works as a timing challenge with a clear win condition. A white bread slice displays with a target shade shown above indicating the goal browning level. Players click the Start button to begin toasting, and the bread gradually browns from white to golden over time. Players must click the Stop button at the right moment to freeze the browning when the bread shade matches the target shade. When the shades match, the game detects the win condition and displays a win message to communicate victory to the player.
