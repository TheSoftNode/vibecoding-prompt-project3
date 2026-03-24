Category: SVG_Generation

Prompt style: Feature_List

Title: Constellation Dot Connector

Prompt: Build a constellation maker that lets users create star patterns by connecting dots. Display an SVG canvas with 8 white dots arranged in a circular pattern on a dark blue background. When users click any dot, change that dot from white to yellow. When users click a second yellow dot, draw a white line connecting the two yellow dots and reset both dots back to white. Include a "Clear All Lines" button below the canvas that removes all drawn lines when clicked.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                                  | Weight | Rationale                                                                                                  | Dependent On |
| --- | ----------- | -------------------------------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display an SVG canvas                                                                        | major  | The SVG canvas provides the space for constellation creation.                                              | None         |
| 2   | visual      | Display dark blue background on SVG canvas                                                   | major  | Dark blue background mimics a night sky for the constellation theme.                                       | C1           |
| 3   | visual      | Display 8 dots on the canvas                                                                 | major  | Eight dots provide connection points for creating constellation patterns.                                  | C1           |
| 4   | visual      | Display dots in white color initially                                                        | major  | White dots represent unselected stars against the night sky.                                               | C3           |
| 5   | layout      | Arrange dots in a circular pattern                                                           | major  | Circular arrangement creates balanced spacing for constellation drawing.                                   | C3           |
| 6   | visual      | Display a "Clear All Lines" button below the canvas                                          | major  | Clear button provides a way to reset the constellation drawing.                                            | None         |
| 7   | interaction | Change dot color from white to yellow when clicked                                           | major  | Yellow color indicates the dot is selected for line drawing.                                               | C3           |
| 8   | interaction | Draw a white line connecting two yellow dots when a second yellow dot is clicked             | major  | Drawing lines creates the constellation pattern between selected stars.                                    | C7           |
| 9   | interaction | Reset both connected dots back to white after drawing the line                               | major  | Resetting dots allows users to select new pairs for additional connections.                                | C8           |
| 10  | state       | Store all drawn lines                                                                        | major  | Storing lines maintains the constellation pattern across interactions.                                     | None         |
| 11  | interaction | Remove all drawn lines when "Clear All Lines" button is clicked                              | major  | Clearing lines lets users start fresh constellation patterns.                                              | C6, C10      |

## Justification

The constellation maker works as a dot-connecting tool for creating star patterns. An SVG canvas displays with a dark blue background representing the night sky. Eight white dots appear arranged in a circular pattern on the canvas. A "Clear All Lines" button displays below the canvas. When users click any dot, that dot changes from white to yellow indicating selection. When users click a second yellow dot, a white line draws connecting the two yellow dots, and both dots reset back to white allowing new selections. The application stores all drawn lines to maintain the constellation pattern. When users click the "Clear All Lines" button, all drawn lines are removed from the canvas.
