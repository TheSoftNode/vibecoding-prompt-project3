Category: Multimedia_Editing

Prompt style: Terse

Title: Split Canvas Mirror Sync

Prompt: Draw on top half, mirrored below. Swap button between halves switches sides. Stroke counter top-left. Undo bottom-left removes last top stroke.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                   | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display canvas split into left and right halves               | major  | Split canvas provides two areas where mirrored drawing occurs.                 | None         |
| 2   | layout      | Position vertical divider at canvas center                    | minor  | Center divider visually separates the two mirrored sides.                      | C1           |
| 3   | interaction | Draw stroke on left side when user drags left half            | major  | Drawing on left creates the original stroke that gets mirrored.                | None         |
| 4   | state       | Track exact coordinates of stroke on left side                | major  | Recording coordinates enables calculating the mirrored position on right side. | C3           |
| 5   | state       | Calculate horizontally flipped coordinates for right side     | major  | Flipping coordinates across center divider creates the mirror effect.          | C4           |
| 6   | interaction | Draw mirrored stroke on right side simultaneously             | major  | Drawing the flipped version on right creates the synchronized mirror.          | C5           |
| 7   | state       | Keep both strokes perfectly synchronized during drag          | major  | Real-time sync ensures mirror appears instantly as user draws.                 | C3, C6       |
| 8   | state       | Track total stroke count across both sides                    | major  | Counting strokes determines when to cycle colors based on every-5 rule.        | C3           |
| 9   | content     | Display stroke count in top-left corner                       | major  | Showing count lets users see how many strokes they've drawn.                   | C8           |
| 10  | layout      | Position stroke count in top-left of canvas                   | minor  | Top-left positioning keeps counter visible without blocking drawing area.      | C9           |
| 11  | state       | Calculate current color from stroke count modulo 2            | major  | Computing color from count divided by 2 determines red or blue phase.          | C8           |
| 12  | visual      | Draw strokes 1-5 in red on both sides                         | major  | Red color for first 5 strokes establishes first phase of cycle.                | C11          |
| 13  | visual      | Draw strokes 6-10 in blue on both sides                       | major  | Blue color for next 5 strokes establishes second phase of cycle.               | C11          |
| 14  | state       | Cycle back to red after every 2 colors complete               | major  | Cycling creates repeating red-blue pattern indefinitely.                       | C11          |
| 15  | visual      | Display undo button                                           | major  | Undo button lets users remove their most recent stroke pair.                   | None         |
| 16  | interaction | Remove last stroke from left side when undo clicked           | major  | Clicking undo deletes the original stroke from left.                           | C15          |
| 17  | interaction | Remove last mirrored stroke from right side when undo clicked | major  | Clicking undo deletes the mirrored stroke from right simultaneously.           | C15          |
| 18  | state       | Decrement stroke count when undo clicked                      | major  | Reducing count keeps counter accurate after removing stroke pair.              | C16, C17     |
| 19  | state       | Update displayed count after decrement                        | major  | Updating display reflects new count after undo.                                | C18          |
| 20  | state       | Recalculate color based on new count after undo               | major  | Recalculating ensures next stroke uses correct color for current count.        | C18          |

## Justification

The Split Canvas Mirror Sync creates real-time mirrored drawing with color cycling and synchronized undo. A canvas displays split into left and right halves with a vertical divider at center. When users drag on the left half, a stroke draws on the left side while tracking exact coordinates. The app calculates horizontally flipped coordinates and draws a mirrored stroke on the right side simultaneously, keeping both strokes perfectly synchronized during the drag. The app tracks total stroke count across both sides and displays this count in the top-left corner. Every 5 strokes, colors cycle between red and blue. Strokes 1-5 draw in red on both sides, strokes 6-10 in blue, then the pattern cycles back to red. Color is calculated from stroke count modulo 2. An undo button removes the last stroke from both left and right sides simultaneously, decrements the stroke count, updates the displayed count, and recalculates the color based on the new count so the next stroke pair uses the correct color.
