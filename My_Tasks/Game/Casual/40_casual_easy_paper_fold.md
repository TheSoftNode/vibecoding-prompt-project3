Category: Game

Prompt style: Casual

Title: Color Square Sorter

Prompt: Show 4 colored squares in row. Display target color order above. Click square to swap with right neighbor. Win message when order matches target.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                    | Weight | Rationale                                                                             | Dependent On |
| --- | ----------- | ---------------------------------------------- | ------ | ------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display 4 colored squares                      | major  | The four colored squares provide the objects players rearrange to match the target.   | None         |
| 2   | layout      | Arrange squares in a row                       | minor  | Row arrangement creates clear left-to-right ordering for the sorting puzzle.          | C1           |
| 3   | content     | Display target color order                     | major  | The target order shows players the goal sequence they must achieve to win.            | None         |
| 4   | layout      | Position target order above squares            | minor  | Above positioning keeps the goal visible while players manipulate squares below.      | C3           |
| 5   | interaction | Swap square with right neighbor when clicked   | major  | Clicking swaps let players rearrange squares to match the target order.               | None         |
| 6   | state       | Update square positions after each swap        | major  | Updating positions shows the current arrangement after each player action.            | C5           |
| 7   | state       | Detect when square order matches target order  | major  | Detection determines when the player has achieved the win condition.                  | C6           |
| 8   | content     | Display win message when order matches target  | major  | The win message communicates victory to the player when the puzzle is solved.         | C7           |

## Justification

The color square sorter game works as a sequencing puzzle with a clear win condition. Four colored squares display arranged in a row. Above them, a target color order displays showing the goal sequence players must achieve. When players click on a square, it swaps positions with its right neighbor, and the square positions update to show the current arrangement. Players continue clicking and swapping until the square order matches the target order. When the arrangement matches the target, the game detects the win condition and displays a win message to communicate victory to the player.
