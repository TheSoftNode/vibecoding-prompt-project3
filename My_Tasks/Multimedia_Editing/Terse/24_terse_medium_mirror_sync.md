Category: Multimedia_Editing

Prompt style: Terse

Title: Split Canvas Mirror Sync

Prompt: Draw on top half; strokes mirror live below. Stroke count (top-left). "Undo" (bottom-left) removes last top stroke. Swap swaps top/bottom content.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                                                     | Weight | Rationale                                                                                                       | Dependent On |
| --- | ----------- | --------------------------------------------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display canvas split into top and bottom halves                                                                 | major  | Showing the split canvas establishes the two drawing areas users need for mirrored drawing.                     | None         |
| 2   | interaction | Draw a stroke on the top half when the user drags the top area                                                  | major  | Letting users draw on top gives them the original stroke that will be mirrored below.                           | None         |
| 3   | state       | Calculate vertically flipped coordinates for the bottom                                                         | major  | Computing flipped coordinates transforms the top stroke position into its mirror on the bottom.                 | None         |
| 4   | interaction | Draw a mirrored stroke on the bottom half simultaneously                                                        | major  | Rendering the mirrored stroke below shows users the real-time mirror effect as they draw.                       | None         |
| 5   | content     | Display text "Undo" on the undo button                                                                          | minor  | Labeling the button "Undo" makes it clear to users that this removes their last stroke.                         | None         |
| 6   | layout      | Position the undo button in the bottom-left of the canvas                                                       | minor  | Placing the undo button in the bottom-left makes it easily accessible to users.                                 | C5           |
| 7   | interaction | Remove only the topmost stroke when Undo is clicked                                                             | major  | Removing only the topmost stroke preserves the bottom mirrored content independently for asymmetric editing.    | None         |
| 8   | content     | Display text "Swap" on the swap button                                                                          | minor  | Labeling the button "Swap" makes it clear to users that this switches content between halves.                   | None         |
| 9   | interaction | Exchange current visible content in top half with current visible content in bottom on each swap button click   | major  | Swapping the top and bottom content gives users a quick way to flip their work and see how different arrangements look from both perspectives. | None         |

## Justification

The Split Canvas Mirror Sync achieved 55.56% pass rate with four failures. A canvas displays split into top and bottom halves. When users drag on the top half, a stroke draws on the top side, and a stroke appears on the bottom side simultaneously. Text "Undo" displays on the undo button. Text "Swap" displays on the swap button. When the swap button is clicked, it exchanges the current visible content in the top half with the current visible content in the bottom. However, the app does not calculate vertically flipped coordinates for the bottom half, so the stroke on the bottom side is an identical copy instead of a vertically mirrored version as required. The undo button is positioned in the top-right area of the header instead of in the bottom-left of the canvas as specified. When the undo button is clicked, it removes the last stroke from both halves instead of removing only the topmost stroke as specified.
