Category: Multimedia_Editing

Prompt style: Terse

Title: Split Canvas Mirror Sync

Prompt: Draw on top half, mirrored below. Swap button swaps content between top and bottom. Stroke counter top-left. Undo bottom-left removes last top stroke.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                             | Weight | Rationale                                                                       | Dependent On |
| --- | ----------- | ------------------------------------------------------- | ------ | ------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display canvas split into top and bottom halves         | major  | Split canvas provides two areas where mirrored drawing occurs.                  | None         |
| 2   | layout      | Position horizontal divider at canvas center            | minor  | Center divider visually separates the two mirrored halves.                      | C1           |
| 3   | interaction | Draw stroke on top half when user drags top area        | major  | Drawing on top creates the original stroke that gets mirrored.                  | None         |
| 4   | state       | Calculate vertically flipped coordinates for bottom     | major  | Flipping coordinates across center creates the mirror effect.                   | C3           |
| 5   | interaction | Draw mirrored stroke on bottom half simultaneously      | minor  | Drawing the flipped version on bottom creates the synchronized mirror.          | C4           |
| 6   | visual      | Display swap button                                     | minor  | Swap button provides the control for swapping content between halves.           | None         |
| 7   | layout      | Position swap button between top and bottom halves      | major  | Positioning swap button between halves makes it accessible for swapping.        | C6           |
| 8   | interaction | Swap top content to bottom when swap button clicked     | major  | Clicking swap moves all top strokes to bottom position.                         | C6           |
| 9   | interaction | Swap bottom content to top when swap button clicked     | major  | Clicking swap moves all bottom strokes to top position simultaneously.          | C6           |
| 10  | content     | Display stroke count                                    | minor  | Showing count lets users see how many strokes they've drawn.                    | C3           |
| 11  | layout      | Position stroke count in top-left of canvas             | major  | Top-left positioning keeps counter in specified location.                       | C10          |
| 12  | visual      | Display undo button                                     | minor  | Undo button lets users remove their most recent stroke.                         | None         |
| 13  | layout      | Position undo button in bottom-left of canvas           | major  | Bottom-left positioning places undo control in specified location.              | C12          |
| 14  | interaction | Remove last stroke from top half when undo clicked      | major  | Clicking undo deletes the original stroke from top only.                        | C12          |
| 15  | state       | Decrement stroke count when undo clicked                | minor  | Reducing count keeps counter accurate after removing stroke.                    | C14          |

## Justification

The Split Canvas Mirror Sync creates real-time mirrored drawing with swap functionality. A canvas displays split into top and bottom halves with a horizontal divider at center. When users drag on the top half, a stroke draws on the top side. The app calculates vertically flipped coordinates and draws a mirrored stroke on the bottom side simultaneously. A swap button positioned between the top and bottom halves allows users to swap all content between the top and bottom positions when clicked. The app displays a stroke count in the top-left corner tracking total strokes drawn. An undo button positioned in the bottom-left corner removes the last stroke from the top half when clicked, decrements the stroke count, and updates the displayed count.
