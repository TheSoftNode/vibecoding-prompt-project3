Category: Multimedia_Editing

Prompt style: Casual

Title: Stroke Merge Editor

Prompt: Draw strokes. Click two to highlight them. Merge combines into one at midpoint. Count shows top-right. Undo splits merge to originals.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                 | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display canvas for drawing strokes                          | major  | Canvas provides the drawing area where users create strokes.                                                     | None         |
| 2   | interaction | Draw stroke when user drags on canvas                       | major  | Dragging creates strokes that can later be selected and merged.                                                  | None         |
| 3   | visual      | Display all drawn strokes on canvas                         | major  | Showing all strokes lets users see which ones are available for selection.                                       | C2           |
| 4   | interaction | Select stroke when user clicks it                           | major  | Clicking a stroke marks it for the merge operation.                                                              | None         |
| 5   | visual      | Highlight first selected stroke                             | major  | Highlighting shows which stroke is selected first.                                                               | C4           |
| 6   | interaction | Select second stroke when user clicks another stroke        | major  | Clicking a second stroke marks the pair for merging.                                                             | C4           |
| 7   | visual      | Highlight second selected stroke                            | major  | Highlighting shows which stroke is selected second, creating a visible pair.                                     | C6           |
| 8   | visual      | Display merge button                                        | major  | Merge button triggers the combination of the two highlighted strokes.                                            | None         |
| 9   | state       | Calculate midpoint between two selected strokes             | major  | Computing midpoint determines where the merged stroke will be positioned.                                        | C4, C6       |
| 10  | interaction | Remove both original strokes when merge clicked             | major  | Clicking merge deletes the two highlighted strokes from canvas.                                                  | C8           |
| 11  | interaction | Create new combined stroke at calculated midpoint           | major  | Creating the merged stroke at midpoint completes the merge operation.                                            | C9, C10      |
| 12  | state       | Store original stroke data for undo functionality           | major  | Storing originals enables splitting the merge back during undo.                                                  | C10          |
| 13  | state       | Track total number of strokes on canvas                     | major  | Counting strokes provides the value to display in the layer counter.                                             | C2, C11      |
| 14  | content     | Display layer count in top-right corner                     | major  | Showing count lets users see how many strokes exist after merges.                                                | C13          |
| 15  | layout      | Position layer count in top-right of canvas                 | minor  | Top-right positioning keeps counter visible without blocking drawing area.                                       | C14          |
| 16  | state       | Update layer count when merge occurs                        | major  | Updating count reflects the reduction from two strokes to one.                                                   | C11          |
| 17  | visual      | Display undo button                                         | major  | Undo button lets users reverse their most recent merge operation.                                                | None         |
| 18  | interaction | Remove merged stroke when undo clicked                      | major  | Clicking undo deletes the combined stroke created by last merge.                                                 | C17          |
| 19  | interaction | Restore both original strokes when undo clicked             | major  | Clicking undo recreates the two strokes that were merged, using stored data.                                     | C12, C18     |
| 20  | state       | Update layer count after undo split                         | major  | Updating count reflects the increase from one merged stroke back to two originals.                               | C19          |

## Justification

The Stroke Merge Editor creates a complex merging system with midpoint calculation and reversible undo. A canvas displays where users can drag to draw strokes. All drawn strokes display on the canvas. Users can click a stroke to select it, which highlights the first selected stroke. Clicking another stroke selects the second one and highlights it, creating a visible pair. A merge button triggers the combination operation. When merge is clicked, the app calculates the midpoint between the two selected strokes, removes both original strokes from canvas, creates a new combined stroke at the calculated midpoint, and stores the original stroke data for undo functionality. The app tracks the total number of strokes on canvas and displays this layer count in the top-right corner, updating the count when merge occurs to reflect the reduction from two strokes to one. An undo button reverses the most recent merge by removing the merged stroke and restoring both original strokes using the stored data, then updating the layer count to reflect the increase from one back to two originals.
