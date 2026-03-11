Category: SVG_Generation

Prompt style: Terse

Title: Star Polygon Generator

Prompt: Generate star polygon in SVG. Input for number of points (5-12). Draw star with specified points in yellow fill, black stroke. Clicking "Regenerate" redraws star with new random rotation angle.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display input field for number of points                 | major  | The input lets users specify how many points their star will have.                                               | None         |
| 2   | content     | Display label indicating points range 5-12               | minor  | Showing the range tells users the valid values they can enter for points.                                        | None         |
| 3   | visual      | Display SVG canvas area                                  | major  | The SVG canvas is where the generated star polygon will be drawn.                                                | None         |
| 4   | visual      | Display star polygon in SVG                              | major  | The star polygon is the main geometric output users are creating.                                                | None         |
| 5   | content     | Display star with yellow fill color                      | minor  | Yellow fill makes the star visually prominent and recognizable.                                                  | None         |
| 6   | content     | Display star with black stroke outline                   | minor  | Black stroke defines the star's edges clearly against any background.                                            | None         |
| 7   | state       | Calculate star points based on input number              | major  | Calculating points from the input value creates the correct star geometry with the specified number of spikes.   | None         |
| 8   | state       | Generate random rotation angle                           | major  | Random rotation makes each regenerated star appear in a different orientation.                                   | None         |
| 9   | visual      | Display "Regenerate" button                              | major  | The Regenerate button provides the control for creating a new star with different rotation.                      | None         |
| 10  | interaction | Redraw star with new rotation when "Regenerate" is clicked | major | Clicking Regenerate creates variation by showing the same star shape at a different angle.                       | C9           |
| 11  | layout      | Position "Regenerate" button below the SVG canvas        | minor  | Placing the button below separates the generation control from the visual output area.                           | None         |

## Justification

The application achieved a 90.91% pass rate with one specific failure. An input field displays with a label indicating the points range 5-12, allowing users to specify the number of star points. An SVG canvas shows a star polygon drawn with yellow fill and black stroke outline. The star's points are calculated based on the input number. A random rotation angle is generated to orient the star. A "Regenerate" button displays on screen. When clicked, it redraws the star with a new random rotation angle while keeping the same number of points, creating different orientations of the same star shape. However, the model failed to position the "Regenerate" button below the SVG canvas. Instead, the button appears to the right of the canvas or above it in a toolbar, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
