Category: Multimedia Editing

Prompt style: Conversational

Title: Image Rotation Editor

Prompt: I need an image rotation tool. When I upload an image, display it on a canvas. Below the canvas, show a slider labeled "Rotation" ranging from 0 to 360 degrees with a default value of 0. As I drag the slider, rotate the image in real-time to match the slider angle and display the current rotation angle in degrees next to the slider.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for image                          | major  | Without an upload button, users can't load their image into the rotation editor.                                 | None         |
| 2   | interaction | Display uploaded image on canvas when file is uploaded   | major  | Showing the image when uploaded provides feedback that the file loaded successfully.                             | C1           |
| 3   | visual      | Display slider control                                   | major  | The slider provides the interface for adjusting rotation angle.                                                  | None         |
| 4   | content     | Display label "Rotation" on slider                       | minor  | Labeling clarifies that the slider controls image rotation angle.                                                | None         |
| 5   | state       | Set slider range from 0 to 360 degrees                   | minor  | The 0-360 range covers a full rotation cycle for the image.                                                      | None         |
| 6   | state       | Set slider default value to 0 degrees                    | minor  | Default 0 means the image starts at its original orientation before rotation.                                    | None         |
| 7   | layout      | Position slider below the canvas                         | minor  | Placing the slider below keeps the rotation control separate from the image display.                             | None         |
| 8   | interaction | Rotate image in real-time when slider is dragged         | major  | Dragging the slider rotates the image immediately, providing the main editing interaction.                       | C3           |
| 9   | content     | Display current rotation angle in degrees next to slider | minor  | Showing the angle value helps users know the exact rotation applied.                                             | None         |
| 10  | layout      | Position angle display next to the slider                | minor  | Placing angle next to slider keeps the rotation value near its control.                                          | None         |

## Justification

The application achieved a 90.00% pass rate with one specific failure. An upload button allows users to load an image, which displays on a canvas when the file is uploaded. A slider labeled "Rotation" with range 0 to 360 degrees appears with a default value of 0. As users drag the slider, the image rotates in real-time. However, the model failed to position the slider below the canvas. Instead, the canvas appears on the left in a two-column layout with the slider controls positioned on the right side, not below the canvas as required. This positioning issue caused the failure despite all other functionality working correctly.
