Category: Game

Prompt style: Casual

Title: Shadow Shape Matcher

Prompt: Need a shape matching puzzle game. At the top, show three empty black outlined boxes arranged side by side: a circular outline, a square outline, and a triangular outline. Below them, display three buttons labeled "Circle", "Square", and "Triangle" in random order on each load. When a user clicks a button, fill the matching outlined box with the corresponding color: red for Circle, blue for Square, and green for Triangle. Keep filled boxes filled.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                    | Weight | Rationale                                                                  | Dependent On |
| --- | ----------- | -------------------------------------------------------------- | ------ | -------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three empty black outlined boxes                       | major  | The outlined boxes show users the target shapes to fill.                   | None         |
| 2   | layout      | Position outlined boxes at the top                             | minor  | Top positioning creates clear visual separation from the buttons.          | C1           |
| 3   | visual      | Show circular outline, square outline, and triangular outline  | major  | The three different shapes identify which box corresponds to each button. | None         |
| 4   | layout      | Arrange the three outlined boxes side by side                  | minor  | Side-by-side arrangement makes it easy to see all three targets.           | C1           |
| 5   | visual      | Display three buttons                                          | major  | The buttons provide the controls for filling the boxes.                    | None         |
| 6   | layout      | Position the three buttons below the outlined boxes            | minor  | Below positioning separates controls from target boxes.                    | C1, C5       |
| 7   | content     | Label the three buttons "Circle", "Square", and "Triangle"     | major  | The labels tell users which button fills which outlined box.               | C5           |
| 8   | state       | Display the three buttons in random order on each load         | minor  | Random order varies the button layout each time for variety.               | C5           |
| 9   | interaction | Fill matching outlined box when corresponding button clicked   | major  | Clicking fills the correct box based on button label matching shape.       | C7           |
| 10  | interaction | Fill circle outline with red when Circle clicked               | major  | Red color provides visual feedback for the circle match.                   | None         |
| 11  | interaction | Fill square outline with blue when Square clicked              | major  | Blue color provides visual feedback for the square match.                  | None         |
| 12  | interaction | Fill triangle outline with green when Triangle clicked         | major  | Green color provides visual feedback for the triangle match.               | None         |
| 13  | state       | Keep filled boxes filled after clicking                        | major  | Maintaining fill state ensures boxes stay colored after interaction completes. | C10, C11, C12 |

## Justification

The Shadow Shape Matcher works as expected with click-to-fill mechanics. Three empty black outlined boxes display at the top arranged side by side: a circular outline, a square outline, and a triangular outline. Below them, three buttons display in random order labeled "Circle", "Square", and "Triangle". When users click the Circle button, the circular outline fills with red and stays filled. When users click the Square button, the square outline fills with blue and stays filled. When users click the Triangle button, the triangular outline fills with green and stays filled.
