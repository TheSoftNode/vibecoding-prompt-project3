Category: Game

Prompt style: Casual

Title: Target Dot Clicker

Prompt: Show 5 target dots. Hover draws path. Click dots to remove. Display hit counter at top. Win when all 5 dots clicked.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                    | Weight | Rationale                                                                             | Dependent On |
| --- | ----------- | ---------------------------------------------- | ------ | ------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display 5 target dots                          | major  | Five target dots provide the objects players must click to win the game.              | None         |
| 2   | visual      | Display path when hovering                     | major  | The drawn path shows where the cursor has been for visual tracking.                   | None         |
| 3   | interaction | Remove target dot when clicked                 | major  | Clicking removes dots, which is the core game mechanic for progressing toward victory.| None         |
| 4   | content     | Display hit counter                            | major  | The hit counter shows how many targets have been clicked.                             | None         |
| 5   | layout      | Position hit counter at top                    | minor  | Top positioning keeps the counter visible throughout gameplay.                        | C4           |
| 6   | state       | Increment hit counter when dot clicked         | major  | Counter increments track the player's progress toward the win condition.              | C3           |
| 7   | state       | Detect when all 5 dots are clicked             | major  | Detection determines when the player has achieved the win condition.                  | C6           |
| 8   | content     | Display win message when all 5 dots clicked    | major  | The win message communicates victory to the player when the game is completed.        | C7           |

## Justification

The shadow path tracer game works as a targeting game with a clear win condition. Five target dots display on screen. When players hover their cursor, a visible path draws showing where the cursor has been for visual tracking. When players click on a target dot, it removes from the screen. A hit counter displays at the top and increments each time a dot is clicked, tracking progress toward victory. When all 5 dots are clicked, the game detects the win condition and displays a win message to communicate victory to the player.
