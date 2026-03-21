Category: Game

Prompt style: Terse

Title: Meteor Catcher

Prompt: Meteors fall from the top when space bar is pressed. Move shield left/right with arrow keys to catch meteors. Show score at top.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                       | Weight | Rationale                                                                 | Dependent On |
| --- | ----------- | ------------------------------------------------- | ------ | ------------------------------------------------------------------------- | ------------ |
| 1   | interaction | Show falling meteor objects when space bar pressed| major  | Space bar trigger starts the meteor fall giving players control of spawn. | None         |
| 2   | state       | Move meteors downward from top continuously       | major  | Moving meteors downward creates the catching challenge.                   | C1           |
| 3   | visual      | Display shield at bottom                    | major  | Showing the shield tells players what catches the meteors.                | None         |
| 4   | layout      | Position shield at bottom of screen         | minor  | Bottom positioning creates the catching zone for the game.                | C3           |
| 5   | interaction | Move shield left when left arrow pressed    | major  | Left arrow lets players position the shield to catch falling meteors.     | None         |
| 6   | interaction | Move shield right when right arrow pressed  | major  | Right arrow lets players position the shield to catch falling meteors.    | None         |
| 7   | state       | Detect when meteor reaches shield position  | major  | Collision detection determines if a meteor was successfully caught.       | C2, C3       |
| 8   | state       | Increment score when meteor caught          | major  | Score increment rewards players for successfully catching meteors.        | C7           |
| 9   | content     | Display score counter                       | minor  | Showing score lets players track their catching performance.              | C8           |
| 10  | layout      | Position score at top of screen             | minor  | Top positioning keeps score visible without blocking the falling meteors. | C9           |

## Justification

The meteor catcher game works as expected for catching gameplay with scoring. When players press the space bar, falling meteor objects appear and move downward from the top continuously. A shield displays positioned at the bottom of the screen. When players press the left arrow key, the shield moves left. When players press the right arrow key, the shield moves right. When a meteor reaches the shield position, the game detects the collision and increments the score. A score counter displays at the top of the screen showing the player's catching performance.
