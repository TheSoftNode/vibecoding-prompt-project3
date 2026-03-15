Category: Game

Prompt style: Casual

Title: Shadow Shape Matcher

Prompt: Need a shape matching puzzle game. At the top, show three empty black outlined boxes arranged side by side: a circular outline, a square outline, and a triangular outline. Below them, load three colorful shapes in random positions that users can drag: a red circle, a blue square, and a green triangle. When a user drags a shape and drops it into its matching outlined box, snap it into place and fill the outlined box with the shape's color. When all three outlined boxes are filled with their matching colors, display "Perfect Match!" in large green text below the shapes.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                    | Weight | Rationale                                                                  | Dependent On |
| --- | ----------- | -------------------------------------------------------------- | ------ | -------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three empty black outlined boxes at the top            | major  | The outlined boxes show users where to place each shape.                   | None         |
| 2   | visual      | Show circular outline, square outline, and triangular outline  | major  | The three different outlines indicate which shape goes where.              | None         |
| 3   | layout      | Arrange the three outlined boxes side by side                  | minor  | Side-by-side arrangement creates clear distinct targets.                   | None         |
| 4   | visual      | Display three colorful shapes below the outlined boxes         | major  | The shapes provide the draggable pieces for the puzzle.                    | None         |
| 5   | visual      | Display red circle, blue square, and green triangle            | major  | The three specific colored shapes match the three outlines.                | None         |
| 6   | state       | Load shapes in random positions                                | major  | Random positioning varies the initial layout each time.                    | None         |
| 7   | interaction | Allow dragging shapes with mouse                               | major  | Dragging lets users move shapes to the outlined boxes.                     | None         |
| 8   | interaction | Snap shape into place when dropped into matching box           | major  | Snapping provides feedback that the shape is correctly placed.             | None         |
| 9   | interaction | Fill outlined box with shape's color when shape placed         | major  | Color filling provides visual confirmation of correct placement.           | None         |
| 10  | content     | Display "Perfect Match!" when all boxes filled                 | major  | The success message rewards users for completing the puzzle.               | None         |
| 11  | visual      | Display message in large green text below shapes               | minor  | Large green text makes the success message prominent and positive.         | None         |

## Justification

The Shadow Shape Matcher works as expected with drag-and-drop puzzle mechanics. Three empty black outlined boxes display at the top arranged side by side: a circular outline, a square outline, and a triangular outline. Below them, three colorful shapes load in random positions: a red circle, a blue square, and a green triangle. When users drag a shape and drop it into its matching outlined box, it snaps into place and fills the outlined box with the shape's color. When all three outlined boxes are filled with their matching colors, "Perfect Match!" displays in large green text below the shapes.
