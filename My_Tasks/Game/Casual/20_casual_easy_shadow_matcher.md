Category: Game

Prompt style: Casual

Title: Shadow Shape Matcher

Prompt: Need a shape matching puzzle game. Show a black filled silhouette target shape at the top. Below it, display three colorful geometric shapes that users can drag with their mouse: a red circle, a blue square, and a green triangle. When a user drags a shape and drops it onto the matching part of the silhouette, snap it into place and keep it there. When all three shapes are correctly placed to complete the silhouette, display "Perfect Match!" in large green text below the shapes. Load a new random silhouette pattern automatically after 2 seconds.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display a black filled silhouette target shape at the top | major  | The silhouette shows users the pattern they need to recreate.                     | None         |
| 2  | layout      | Position silhouette at the top of the display            | minor  | Top positioning creates clear visual separation between target and shapes.         | C1           |
| 3  | visual      | Display three colorful geometric shapes below silhouette | major  | The shapes provide the draggable pieces for the puzzle.                            | None         |
| 4  | visual      | Display red circle as one draggable shape                | minor  | The red circle is one of the three pieces users can manipulate.                    | C3           |
| 5  | visual      | Display blue square as one draggable shape               | minor  | The blue square is one of the three pieces users can manipulate.                   | C3           |
| 6  | visual      | Display green triangle as one draggable shape            | minor  | The green triangle is one of the three pieces users can manipulate.                | C3           |
| 7  | interaction | Allow dragging shapes with mouse                         | major  | Dragging lets users move shapes to match the silhouette.                           | None         |
| 8  | interaction | Snap shape into place when dropped on matching silhouette part | major  | Snapping provides visual feedback that the shape is correctly positioned.          | None         |
| 9  | state       | Keep shape in place after correct drop                   | major  | Keeping shapes placed maintains the puzzle progress toward completion.             | C8           |
| 10 | content     | Display "Perfect Match!" when all shapes placed correctly | major  | The success message rewards users for completing the puzzle.                       | None         |
| 11 | visual      | Display message in large green text below shapes         | minor  | Large green text makes the success message prominent and positive.                 | C10          |
| 12 | state       | Load new random silhouette pattern after 2 seconds       | major  | Auto-loading keeps the game progressing with fresh challenges.                     | None         |

## Justification

The Shadow Shape Matcher works as expected with drag-and-drop puzzle mechanics. A black filled silhouette target shape displays at the top of the screen. Below it, three colorful geometric shapes appear that users can drag: a red circle, a blue square, and a green triangle. When users drag a shape and drop it onto the matching part of the silhouette, it snaps into place and stays there. When all three shapes are correctly placed to complete the silhouette, "Perfect Match!" displays in large green text below the shapes. A new random silhouette pattern loads automatically after 2 seconds.
