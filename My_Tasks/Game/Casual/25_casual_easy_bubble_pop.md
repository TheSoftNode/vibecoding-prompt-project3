Category: Game

Prompt style: Casual

Title: Bubble Chain Popper

Prompt: Need a bubble popping game. Show 6 bubbles floating on screen, each labeled with a letter A through F. When I click a bubble, it pops and disappears with a visual effect. Display a "Pop Count" at the bottom tracking how many bubbles I've popped. When all 6 bubbles are popped, show "All Clear!" message and a "New Round" button that respawns all bubbles.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 6 bubbles on screen                          | major  | Showing bubbles gives players the targets they need to pop.                                  | None         |
| 2   | content     | Label each bubble with letters A through F           | major  | Labeling bubbles identifies each one uniquely so players can distinguish them.               | C1           |
| 3   | layout      | Position bubbles scattered across screen             | minor  | Scattering bubbles creates the floating visual appearance for the popping game.              | C1           |
| 4   | interaction | Detect bubble click from player                      | major  | Detecting clicks captures which bubble the player wants to pop.                              | C1           |
| 5   | visual      | Display visual effect when bubble clicked            | major  | Showing pop effect gives satisfying feedback that the bubble was successfully clicked.       | C4           |
| 6   | interaction | Remove bubble from screen after click                | major  | Removing bubble shows the popping action was completed and that bubble is gone.              | C4           |
| 7   | visual      | Display "Pop Count" label                            | minor  | Showing label tells players what the number below it represents.                             | None         |
| 8   | layout      | Position "Pop Count" at bottom of screen             | minor  | Placing count at bottom keeps it visible without blocking the bubbles above.                 | C7           |
| 9   | state       | Increment count by 1 when bubble removed             | major  | Incrementing count tracks how many bubbles the player has successfully popped so far.        | C6           |
| 10  | content     | Display current pop count number                     | major  | Showing number tells players how many bubbles they have popped.                              | C9           |
| 11  | state       | Detect when all 6 bubbles are removed                | major  | Detecting completion determines when the player finished popping every bubble.               | C6           |
| 12  | content     | Display "All Clear!" message when all removed        | major  | Showing message tells players they successfully popped all bubbles and completed the round.  | C11          |
| 13  | visual      | Display "New Round" button when all removed          | major  | Showing button gives players the control to start another popping round.                     | C11          |
| 14  | interaction | Respawn all 6 bubbles when "New Round" clicked       | major  | Clicking button creates fresh bubbles so players can pop them again in a new round.          | C13          |

## Justification

The bubble chain popper game works as expected for simple clicking gameplay with round completion. Six bubbles display on screen positioned scattered across the interface, each labeled with letters A through F. A "Pop Count" label displays positioned at the bottom of the screen with the current pop count number showing how many bubbles have been popped. When players click a bubble, the game detects the click, displays a visual effect, removes the bubble from the screen, increments the count by 1, and displays the updated pop count number. When all 6 bubbles are removed, the game detects completion, displays "All Clear!" message, and displays a "New Round" button. When players click the "New Round" button, all 6 bubbles respawn on screen.
