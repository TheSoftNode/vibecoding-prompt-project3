Category: Multimedia_Editing

Prompt style: Terse

Title: Split Canvas Mirror Sync

Prompt: Draw on top half, mirrored below. Swap button swaps content between top and bottom. Stroke counter top-left. Undo bottom-left removes last top stroke.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                             | Weight | Rationale                                                                                          | Dependent On |
| --- | ----------- | ------------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display canvas split into top and bottom halves         | major  | Showing the split canvas establishes the two drawing areas users need for mirrored drawing.        | None         |
| 2   | layout      | Position horizontal divider at canvas center            | minor  | Centering the divider creates equal space for both top and bottom drawing areas.                   | C1           |
| 3   | interaction | Draw stroke on top half when user drags top area        | major  | Letting users draw on top gives them the original stroke that will be mirrored below.              | None         |
| 4   | state       | Calculate vertically flipped coordinates for bottom     | major  | Computing flipped coordinates transforms the top stroke position into its mirror on the bottom.    | C3           |
| 5   | interaction | Draw mirrored stroke on bottom half simultaneously      | minor  | Rendering the mirrored stroke below shows users the real-time mirror effect as they draw.          | C4           |
| 6   | visual      | Display swap button                                     | minor  | Showing the swap button gives users a visible control for switching content between halves.        | None         |
| 7   | layout      | Position swap button between top and bottom halves      | major  | Placing swap button between halves makes its purpose clear and keeps it accessible for clicking.   | C6           |
| 8   | interaction | Swap top content to bottom when swap button clicked     | major  | Moving top strokes to bottom lets users flip their drawing to the other half.                      | C6           |
| 9   | interaction | Swap bottom content to top when swap button clicked     | major  | Moving bottom strokes to top completes the swap so both halves exchange content simultaneously.    | C6           |
| 10  | content     | Display stroke count                                    | minor  | Showing the count tells users how many strokes they have drawn so far.                             | C3           |
| 11  | layout      | Position stroke count in top-left of canvas             | major  | Placing count in top-left keeps it visible without blocking the drawing area.                      | C10          |
| 12  | visual      | Display undo button                                     | minor  | Showing the undo button gives users a visible control for removing their last stroke.              | None         |
| 13  | layout      | Position undo button in bottom-left of canvas           | major  | Placing undo in bottom-left keeps it accessible while separating it from the stroke counter.       | C12          |
| 14  | interaction | Remove last stroke from top half when undo clicked      | major  | Deleting the last top stroke lets users correct their most recent drawing mistake.                 | C12          |
| 15  | state       | Decrement stroke count when undo clicked                | minor  | Reducing the count after undo keeps the displayed number accurate with actual strokes remaining.   | C14          |

## Justification

The Split Canvas Mirror Sync creates real-time mirrored drawing with swap functionality. A canvas displays split into top and bottom halves with a horizontal divider at center. When users drag on the top half, a stroke draws on the top side. The app calculates vertically flipped coordinates and draws a mirrored stroke on the bottom side simultaneously. A swap button positioned between the top and bottom halves allows users to swap all content between the top and bottom positions when clicked. The app displays a stroke count in the top-left corner tracking total strokes drawn. An undo button positioned in the bottom-left corner removes the last stroke from the top half when clicked, decrements the stroke count, and updates the displayed count.
