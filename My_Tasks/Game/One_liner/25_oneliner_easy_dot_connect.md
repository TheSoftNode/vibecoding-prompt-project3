Category: Game

Prompt style: One_liner

Title: Dot Connection Game

Prompt: Click dots to connect them in order 1→2→3→4→5, wrong order shows red flash, correct completion shows "Win!" message.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 5 dots on screen                             | major  | Showing dots gives players the objects they need to connect.                                 | None         |
| 2   | content     | Label dots with numbers 1, 2, 3, 4, 5                | major  | Showing numbers tells players the correct connection sequence.                               | C1           |
| 3   | layout      | Position dots scattered on screen                    | minor  | Scattering dots creates the connection challenge for players.                                | C1           |
| 4   | interaction | Detect dot clicks from player                        | major  | Detecting clicks captures the connection sequence players attempt.                           | C1           |
| 5   | state       | Track click order in sequence                        | major  | Tracking order determines if the player is connecting dots correctly.                        | C4           |
| 6   | state       | Check if clicked dot is next in correct sequence     | major  | Checking sequence validates whether the player clicked the right dot.                        | C5           |
| 7   | visual      | Show red flash when wrong dot clicked                | major  | Flashing red gives immediate feedback that the player clicked out of order.                  | C6           |
| 8   | state       | Continue accepting clicks after wrong order          | major  | Allowing continued play lets players try again without restarting.                           | C7           |
| 9   | state       | Detect when all 5 dots connected in order 1→2→3→4→5  | major  | Checking completion determines when the player successfully finished the sequence.           | C6           |
| 10  | content     | Display "Win!" message when sequence complete        | major  | Showing win message tells players they successfully connected all dots in order.             | C9           |
| 11  | interaction | Disable further clicking after win                   | major  | Disabling clicks prevents additional connections after the challenge is complete.            | C9           |
| 12  | visual      | Draw connecting lines between clicked dots           | minor  | Showing lines visualizes the connection path the player has made.                            | C5           |

## Justification

The dot connection game works as expected for sequential clicking gameplay. Five dots display on screen labeled with numbers 1, 2, 3, 4, 5, positioned scattered across the interface. When players click a dot, the game detects the click and tracks the click order in sequence. The game checks if the clicked dot is next in the correct sequence (1→2→3→4→5). If the player clicks the wrong dot, it shows a red flash but continues accepting clicks so players can try again. When all 5 dots are connected in the correct order 1→2→3→4→5, the game detects completion, displays "Win!" message, and disables further clicking.
