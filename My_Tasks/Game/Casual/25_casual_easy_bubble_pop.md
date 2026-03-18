Category: Game

Prompt style: Casual

Title: Bubble Chain Popper

Prompt: Need a bubble popping game. Show 6 bubbles floating on screen, each labeled with a letter A through F. When I click a bubble, it pops and disappears with a visual effect. Display a "Pop Count" at the bottom tracking how many bubbles I've popped. When all 6 bubbles are popped, show "All Clear!" message and a "New Round" button that respawns all bubbles.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 6 bubbles floating on screen                 | major  | Showing bubbles gives players the targets they need to pop.                                  | None         |
| 2   | content     | Label each bubble with letters A through F           | major  | Labeling bubbles identifies each one uniquely so players can distinguish them.               | C1           |
| 3   | layout      | Position bubbles scattered across screen             | minor  | Scattering bubbles creates a floating appearance for the popping game.                       | C1           |
| 4   | interaction | Pop bubble when clicked                              | major  | Clicking bubble triggers the popping action players expect.                                  | C1           |
| 5   | visual      | Display visual effect when bubble pops               | major  | Showing effect gives satisfying feedback that the bubble was successfully popped.            | C4           |
| 6   | interaction | Remove bubble from screen after popping              | major  | Removing bubble shows the popping action was registered and changes game state.              | C4           |
| 7   | content     | Display "Pop Count" at the bottom                    | minor  | Showing count label tells players what the number represents.                                | None         |
| 8   | state       | Increment count when bubble is popped                | major  | Incrementing count tracks how many bubbles the player has successfully popped.               | C6           |
| 9   | content     | Update displayed count after each pop                | major  | Updating display shows players their popping progress in real time.                          | C8           |
| 10  | state       | Detect when all 6 bubbles are popped                 | major  | Detecting completion determines when the round is finished.                                  | C6           |
| 11  | content     | Display "All Clear!" message when all popped         | major  | Showing completion message tells players they finished popping all bubbles.                  | C10          |
| 12  | visual      | Display "New Round" button after all popped          | major  | Showing button gives players control to start another round.                                 | C10          |
| 13  | interaction | Respawn all 6 bubbles when "New Round" clicked       | major  | Clicking button restarts the game with fresh bubbles for another popping round.              | C12          |

## Justification

The bubble chain popper game works as expected for simple clicking gameplay with round completion. Six bubbles display floating on screen, scattered across the interface, each labeled with letters A through F. When players click a bubble, it pops with a visual effect and disappears from the screen. A "Pop Count" displays at the bottom and increments each time a bubble is popped, updating the display in real time. When all 6 bubbles are popped, the game detects completion, displays "All Clear!" message, and shows a "New Round" button. When players click the "New Round" button, all 6 bubbles respawn on screen.
