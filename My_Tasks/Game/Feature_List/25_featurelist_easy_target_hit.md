Category: Game

Prompt style: Feature_List

Title: Target Hit Tracker

Prompt: Build a target hitting game with these features: Display 5 circular targets labeled "T1", "T2", "T3", "T4", "T5" spread across the screen. Each target starts with a white background. When players click a target, change its background to green and mark it as hit. Display a timer labeled "Time: 0s" at the top-left that starts counting seconds from 0 when the first target is clicked and stops when all 5 targets are hit. Display a "Reset" button at the bottom that returns all targets back to white background and resets the timer to 0 when clicked, allowing players to start a fresh hitting session.

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
| 7   | content     | Display timer labeled "Time: 0s"                     | major  | Showing timer tells players how long they're taking to hit all targets.                      | None         |
| 8   | layout      | Position timer at top-left                           | minor  | Top-left positioning keeps timer visible while players hit targets.                          | C7           |
| 9   | interaction | Start timer counting when first target clicked       | major  | Clicking first target starts the timer to begin tracking hitting speed.                      | C5           |
| 10  | state       | Count seconds from 0 and update displayed time       | major  | Counting seconds tracks how long the player takes to hit all targets.                        | C9           |
| 11  | state       | Detect when all 5 targets are hit                    | major  | Detecting completion determines when to stop the timer.                                      | C6           |
| 12  | interaction | Stop timer when all 5 targets are hit                | major  | Stopping timer captures the final completion time for the hitting session.                   | C11          |
| 13  | visual      | Display Reset button                                 | major  | Showing button gives players control to restart the hitting challenge.                       | None         |
| 14  | layout      | Position Reset button at bottom                      | minor  | Bottom positioning keeps the reset control separate from gameplay elements.                  | C13          |
| 15  | interaction | Return all targets to white and reset timer to 0 when Reset clicked | major  | Clicking reset clears all hit markers and timer for a fresh hitting session.                 | C13          |

## Justification

The target hit tracker game works exactly as expected for clicking gameplay with timer tracking. Five circular targets display spread across the screen, each labeled "T1", "T2", "T3", "T4", "T5" with white backgrounds initially. A timer labeled "Time: 0s" displays positioned at the top-left. When players click the first target, the timer starts counting seconds from 0 and updates the displayed time. When players click targets, each target changes its background to green and marks as hit. When all 5 targets are hit, the game detects completion and stops the timer. A Reset button displays at the bottom. When players click the Reset button, all targets return to white backgrounds and the timer resets to 0, allowing a fresh hitting session.
