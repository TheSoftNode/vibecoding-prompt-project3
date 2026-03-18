Category: Multimedia_Editing

Prompt style: Casual

Title: Gravity Dot Animator

Prompt: Click spawns dot. Dots fall downward until hitting canvas bottom or another dot. Stack height shows top-left. Clear button bottom-right removes all and resets height. Pause button top-right freezes falling dots.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                         | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | --------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display canvas for dot animation                    | major  | Canvas provides the area where dots spawn and fall with gravity.               | None         |
| 2   | interaction | Spawn dot at click position when user clicks canvas | major  | Clicking creates dots that will fall with gravity simulation.                  | None         |
| 3   | state       | Apply downward velocity to spawned dot              | major  | Downward velocity makes dots fall realistically toward bottom.                 | C2           |
| 4   | state       | Animate dot falling continuously until collision    | minor  | Continuous animation creates the falling motion effect.                        | C3           |
| 5   | state       | Detect when dot reaches canvas bottom edge          | minor  | Bottom detection determines when dot should stop falling.                      | C4           |
| 6   | state       | Detect when dot collides with another dot           | minor  | Dot collision detection determines when falling dot hits stationary dot.       | C4           |
| 7   | state       | Stop dot movement when bottom edge reached          | minor  | Stopping at bottom prevents dots from falling off canvas.                      | C5           |
| 8   | state       | Stop dot movement when collision with dot occurs    | minor  | Stopping on collision creates stacking behavior where dots pile up.            | C6           |
| 9   | content     | Display stack height                                | minor  | Showing height lets users see how tall their dot stack has grown.              | None         |
| 10  | layout      | Position stack height in top-left of canvas         | major  | Top-left positioning keeps measurement in specified location.                  | C9           |
| 11  | visual      | Display clear button                                | minor  | Clear button lets users reset the animation and start fresh.                   | None         |
| 12  | layout      | Position clear button in bottom-right of canvas     | major  | Bottom-right positioning places clear control in specified corner.             | C11          |
| 13  | interaction | Remove all dots when clear button clicked           | major  | Clicking clear deletes all dots from canvas.                                   | C11          |
| 14  | interaction | Reset stack height to zero when clear clicked       | major  | Resetting height to zero keeps measurement accurate after clearing.            | C13          |
| 15  | visual      | Display pause button                                | minor  | Pause button lets users freeze the falling animation.                          | None         |
| 16  | layout      | Position pause button in top-right of canvas        | major  | Top-right positioning places pause control in specified corner.                | C15          |
| 17  | interaction | Freeze falling dots when pause button clicked       | major  | Clicking pause stops all dot movement mid-fall.                                | C15          |
| 18  | interaction | Resume falling dots when pause button clicked again | major  | Clicking pause again continues dot animation from frozen state.                | C17          |

## Justification

The Gravity Dot Animator creates a physics-based stacking simulation with height tracking, pause control, and clear functionality. A canvas displays where dots spawn and animate. When users click the canvas, a dot spawns at the click position with downward velocity applied. The dot animates falling continuously until it reaches the canvas bottom edge or collides with another dot, then stops movement. Stack height displays in the top-left corner. A clear button positioned in the bottom-right corner removes all dots when clicked and resets the stack height to zero. A pause button positioned in the top-right corner freezes all falling dots when clicked and resumes the falling animation when clicked again.
