Category: Multimedia_Editing

Prompt style: One-liner

Title: Stamping Grid Counter

Prompt: Click to stamp circles in 4x4 grid snapping to nearest empty slot, count shows top-center incrementing per stamp, reset clears all.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                 | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display canvas with 4x4 grid layout                         | major  | The grid provides the structured positions where stamps can be placed.                                           | None         |
| 2   | layout      | Position 16 grid slots in 4 rows and 4 columns              | major  | 4x4 arrangement creates the specific grid structure with 16 possible stamp positions.                            | C1           |
| 3   | interaction | Stamp circle when user clicks canvas                        | major  | Clicking creates stamps so users can fill the grid positions.                                                    | None         |
| 4   | state       | Calculate nearest empty grid slot to click position         | major  | Finding the nearest empty slot determines which grid position receives the stamp.                                | C3           |
| 5   | state       | Snap stamp to calculated grid position                      | major  | Snapping ensures stamps align to grid slots instead of appearing at raw click coordinates.                       | C4           |
| 6   | state       | Prevent stamping in already-filled grid slots               | major  | Blocking filled slots ensures each grid position holds only one stamp.                                           | C4           |
| 7   | visual      | Display all stamped circles in their grid positions         | major  | Showing all stamps lets users see which grid slots they've filled.                                               | C5           |
| 8   | state       | Track total number of stamps placed                         | major  | Counting stamps provides the value to display in the stamp counter.                                              | C3           |
| 9   | content     | Display stamp count in top-center of canvas                 | major  | Showing the count lets users see how many stamps they've placed.                                                 | C8           |
| 10  | layout      | Position stamp count at top-center                          | minor  | Top-center positioning keeps the counter visible and centered above the grid.                                    | C9           |
| 11  | state       | Increment stamp count by 1 for each stamp placed            | major  | Incrementing count keeps the counter accurate as users add stamps.                                               | C3           |
| 12  | state       | Update displayed count after each increment                 | major  | Updating the display reflects the new count after each stamp.                                                    | C11          |
| 13  | visual      | Display reset button                                        | major  | The reset button lets users clear the grid and start over.                                                       | None         |
| 14  | interaction | Remove all stamps when reset button clicked                 | major  | Clicking reset deletes all stamps from the grid.                                                                 | C13          |
| 15  | state       | Reset stamp count to zero when reset clicked                | major  | Resetting count to zero keeps the counter accurate after clearing.                                               | C14          |
| 16  | state       | Update displayed count to show zero after reset             | major  | Updating the display reflects the reset state after clearing the grid.                                           | C15          |
| 17  | state       | Mark all grid slots as empty after reset                    | major  | Marking slots empty allows users to stamp in any position again after reset.                                     | C14          |

## Justification

The Stamping Grid Counter creates a structured stamping system with snapping, counting, and reset functionality. A canvas displays with a 4x4 grid layout containing 16 grid slots arranged in 4 rows and 4 columns. When users click the canvas, the app calculates the nearest empty grid slot to the click position and snaps the stamp to that grid position instead of the raw click coordinates. Each click stamps a circle in the snapped position, preventing stamping in already-filled slots so each grid position holds only one stamp. The app tracks the total number of stamps placed and displays this count at the top-center of the canvas, incrementing by 1 for each stamp and updating the display after each increment. All stamped circles display in their grid positions. A reset button removes all stamps from the grid, marks all grid slots as empty, resets the stamp count to zero, and updates the displayed count to show zero.
