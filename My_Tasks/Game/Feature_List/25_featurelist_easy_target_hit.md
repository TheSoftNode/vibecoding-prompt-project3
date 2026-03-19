Category: Game

Prompt style: Feature_List

Title: Target Hit Tracker

Prompt: Build a target hitting game with these features: Display 5 circular targets labeled "T1", "T2", "T3", "T4", "T5" spread across the screen. Each target starts with a white background. When players click a target, change its background to green and mark it as hit. Display a hit counter labeled "Hits: 0" at the top-left that shows the total number of targets hit. Display a "Reset" button at the bottom that returns all targets back to white background and resets the hit counter to 0 when clicked, allowing players to start a fresh hitting session.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 5 circular targets                           | major  | Showing targets gives players the objects they need to hit.                                  | None         |
| 2   | content     | Label targets "T1", "T2", "T3", "T4", "T5"           | major  | Showing labels identifies each target uniquely for players.                                  | C1           |
| 3   | layout      | Spread targets across screen                         | minor  | Spreading targets creates distributed hitting challenge for players.                         | C1           |
| 4   | visual      | Show each target with white background initially     | major  | Starting white establishes the unhit state that players will change.                         | C1           |
| 5   | interaction | Change target background to green when clicked       | major  | Clicking target changes its color showing the hitting action was registered.                 | C1           |
| 6   | state       | Mark target as hit when clicked                      | major  | Marking as hit tracks which targets the player has successfully clicked.                     | C5           |
| 7   | content     | Display hit counter labeled "Hits: 0"                | major  | The hit counter shows players how many targets they've successfully hit.                     | None         |
| 8   | layout      | Position hit counter at top-left                     | minor  | Top-left positioning keeps the counter visible while players hit targets.                    | C7           |
| 9   | state       | Increment hit counter when target clicked            | major  | Incrementing the counter tracks the total number of targets hit.                             | C5           |
| 10  | content     | Update displayed hit count after each click          | major  | Updating the display shows the current hit count in real time.                               | C9           |
| 11  | visual      | Display Reset button                                 | major  | Showing button gives players control to restart the hitting challenge.                       | None         |
| 12  | layout      | Position Reset button at bottom                      | minor  | Bottom positioning keeps the reset control separate from gameplay elements.                  | C11          |
| 13  | interaction | Return all targets to white and reset counter to 0 when Reset clicked | major  | Clicking reset clears all hit markers and counter for a fresh hitting session.               | C11          |

## Justification

The target hit tracker game works exactly as expected for clicking gameplay with hit counting. Five circular targets display spread across the screen, each labeled "T1", "T2", "T3", "T4", "T5" with white backgrounds initially. A hit counter labeled "Hits: 0" displays positioned at the top-left. When players click a target, that target changes its background to green, marks as hit, and the hit counter increments with the updated count displayed. A Reset button displays at the bottom. When players click the Reset button, all targets return to white backgrounds and the hit counter resets to 0, allowing a fresh hitting session.
