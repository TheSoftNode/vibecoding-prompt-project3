Category: Game

Prompt style: Feature_List

Title: Target Hit Tracker

Prompt: Build a target hitting game with these features: Display 5 circular targets labeled "T1", "T2", "T3", "T4", "T5" spread across the screen. Each target starts with a white background. When players click a target, change its background to green and mark it as hit. Display a hit counter labeled "Hits: 0" at the top-left that increments each time a target is clicked. Display a "Reset" button at the bottom that returns all targets to white and resets the hit counter to zero when clicked.

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
| 7   | content     | Display hit counter labeled "Hits: 0"                | major  | Showing counter tells players how many targets they've successfully hit.                     | None         |
| 8   | layout      | Position hit counter at top-left                     | minor  | Top-left positioning keeps counter visible while players hit targets.                        | C7           |
| 9   | interaction | Detect each target click                             | major  | Detecting clicks captures player hitting actions for counting and marking.                   | C1           |
| 10  | state       | Increment hit counter when target clicked            | major  | Incrementing count tracks the total number of targets the player has hit.                    | C9           |
| 11  | content     | Update displayed hit count after each click          | major  | Updating display shows players their hitting progress in real time.                          | C10          |
| 12  | visual      | Display Reset button at bottom                       | major  | Showing button gives players control to restart the hitting challenge.                       | None         |
| 13  | interaction | Return all targets to white when Reset clicked       | major  | Clicking reset clears all hit markers returning targets to unhit state.                      | C12          |
| 14  | interaction | Reset hit counter to zero when Reset clicked         | major  | Clicking reset clears the count so players can track a fresh hitting session.               | C12          |

## Justification

The target hit tracker game works as expected for clicking gameplay with reset functionality. Five circular targets display spread across the screen, each labeled "T1", "T2", "T3", "T4", "T5" with white backgrounds initially. A hit counter labeled "Hits: 0" displays positioned at the top-left. When players click a target, the game detects the click, changes the target's background to green, marks it as hit, increments the hit counter, and updates the displayed count. A Reset button displays at the bottom. When players click the Reset button, all targets return to white backgrounds and the hit counter resets to zero.
