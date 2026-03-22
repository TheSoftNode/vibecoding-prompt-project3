Category: Game

Prompt style: Casual

Title: Bubble Chain Popper

Prompt: Click bubbles to pop them. Popped bubbles make nearby bubbles grow bigger. Show pop count at top.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                      | Weight | Rationale                                                                  | Dependent On |
| --- | ----------- | ------------------------------------------------ | ------ | -------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display bubble objects                           | major  | Showing bubbles gives players the targets they need to pop.                | None         |
| 2   | interaction | Pop bubble when clicked                          | major  | Clicking pops a bubble to start the chain reaction.                        | None         |
| 3   | visual      | Show pop effect on clicked bubble                | major  | Pop effect shows which bubble was clicked.                                 | C2           |
| 4   | state       | Make nearby bubbles grow bigger when bubble pops | major  | Growing nearby bubbles creates the chain reaction mechanic.                | C2           |
| 5   | visual      | Show growth effect on nearby bubbles             | major  | Growth effect shows which bubbles were affected by the pop.                | C4           |
| 6   | content     | Display pop count                                | minor  | Showing count gives users feedback on how many bubbles they popped.        | None         |
| 7   | layout      | Position pop count at top of screen              | minor  | Top positioning keeps count visible without blocking the bubbles.          | C6           |
| 8   | state       | Increment pop count when bubble clicked          | major  | Counting each pop tracks the player's performance.                         | C2           |

## Justification

The bubble chain popper game works as expected for chain reaction gameplay with scoring. Bubble objects display on screen. When players click a bubble, it pops showing a pop effect. Nearby bubbles grow bigger showing a growth effect creating the chain reaction. A pop count displays at the top of the screen and increments each time a bubble is clicked tracking the player's popping performance.
