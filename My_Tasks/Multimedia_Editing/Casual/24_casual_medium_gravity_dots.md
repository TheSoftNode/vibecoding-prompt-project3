Category: Multimedia_Editing

Prompt style: Casual

Title: Gravity Dot Animator

Prompt: Click spawns dot. Dots fall downward until hitting canvas bottom or another dot. Stack height shows top-right. Clear removes all and resets height.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                 | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display canvas for dot animation                            | major  | Canvas provides the area where dots spawn and fall with gravity.                                                 | None         |
| 2   | interaction | Spawn dot at click position when user clicks canvas         | major  | Clicking creates dots that will fall with gravity simulation.                                                    | None         |
| 3   | state       | Apply downward velocity to spawned dot                      | major  | Downward velocity makes dots fall realistically toward bottom.                                                   | C2           |
| 4   | state       | Animate dot falling continuously until collision            | major  | Continuous animation creates the falling motion effect.                                                          | C3           |
| 5   | state       | Detect when dot reaches canvas bottom edge                  | major  | Bottom detection determines when dot should stop falling.                                                        | C4           |
| 6   | state       | Detect when dot collides with another dot                   | major  | Dot collision detection determines when falling dot hits stationary dot.                                         | C4           |
| 7   | state       | Stop dot movement when bottom edge reached                  | major  | Stopping at bottom prevents dots from falling off canvas.                                                        | C5           |
| 8   | state       | Stop dot movement when collision with dot occurs            | major  | Stopping on collision creates stacking behavior where dots pile up.                                              | C6           |
| 9   | state       | Position stopped dot resting on collision surface           | major  | Positioning on surface makes dots stack vertically on top of each other.                                         | C8           |
| 10  | visual      | Display all dots in their final resting positions           | major  | Showing all dots creates the visible stack of accumulated dots.                                                  | C7, C9       |
| 11  | state       | Calculate maximum vertical stack height from bottom         | major  | Computing height from bottom edge to topmost dot determines stack measurement.                                   | C9           |
| 12  | content     | Display stack height value in top-right corner              | major  | Showing height lets users see how tall their dot stack has grown.                                                | C11          |
| 13  | layout      | Position stack height in top-right of canvas                | minor  | Top-right positioning keeps measurement visible without blocking animation.                                      | C12          |
| 14  | state       | Update height display when new dot stops                    | major  | Updating height after each dot settles keeps measurement accurate.                                               | C11          |
| 15  | visual      | Display clear button                                        | major  | Clear button lets users reset the animation and start fresh.                                                     | None         |
| 16  | interaction | Remove all dots when clear button clicked                   | major  | Clicking clear deletes all dots from canvas.                                                                     | C15          |
| 17  | state       | Reset stack height to zero when clear clicked               | major  | Resetting height to zero keeps measurement accurate after clearing.                                              | C16          |
| 18  | state       | Update displayed height to show zero after clear            | major  | Updating display reflects reset state after clearing canvas.                                                     | C17          |

## Justification

The Gravity Dot Animator creates a physics-based stacking simulation with height tracking and clear functionality. A canvas displays where dots spawn and animate. When users click the canvas, a dot spawns at the click position with downward velocity applied. The dot animates falling continuously until collision occurs. The app detects when the dot reaches the canvas bottom edge or collides with another dot. When bottom edge is reached, the dot stops movement. When collision with another dot occurs, the dot stops and positions itself resting on the collision surface, creating vertical stacking behavior where dots pile up on top of each other. All dots display in their final resting positions showing the accumulated stack. The app calculates maximum vertical stack height from the bottom edge to the topmost dot and displays this height value in the top-right corner. The height display updates when each new dot stops. A clear button removes all dots from the canvas, resets the stack height to zero, and updates the displayed height to show zero.
