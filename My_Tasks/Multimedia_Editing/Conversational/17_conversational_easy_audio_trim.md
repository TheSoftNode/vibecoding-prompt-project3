Category: Multimedia Editing

Prompt style: Conversational

Title: Image Rotation Editor

Prompt: I need an image rotation tool. When I upload an image, display it on a canvas. Below the canvas, show a slider labeled "Rotation" ranging from 0 to 360 degrees with a default value of 0. As I drag the slider, rotate the image in real-time to match the slider angle and display the current rotation angle in degrees next to the slider.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for image                          | major  | Without an upload button, users can't load their image into the rotation editor.                                 | None         |
| 2   | visual      | Display uploaded image on canvas                         | major  | The canvas shows the image so users can see the rotation effect.                                                 | None         |
| 3   | visual      | Display slider control                                   | major  | The slider provides the interface for adjusting rotation angle.                                                  | None         |
| 4   | content     | Display label "Rotation" on slider                       | minor  | Labeling clarifies that the slider controls image rotation angle.                                                | None         |
| 5   | content     | Display slider range from 0 to 360 degrees               | minor  | Showing the range tells users they can rotate a full 360 degrees.                                                | None         |
| 6   | state       | Set slider default value to 0 degrees                    | minor  | Default 0 means the image starts at its original orientation before rotation.                                    | None         |
| 7   | layout      | Position slider below the canvas                         | minor  | Placing the slider below keeps the rotation control separate from the image display.                             | None         |
| 8   | state       | Store current rotation angle from slider                 | major  | Storing the angle is necessary to apply the correct rotation to the image.                                       | None         |
| 9   | interaction | Rotate image when slider is dragged                      | major  | Dragging the slider rotates the image, providing the main editing interaction.                                   | C3           |
| 10  | state       | Apply rotation in real-time as slider moves              | major  | Real-time rotation lets users see the effect immediately while dragging.                                         | None         |
| 11  | content     | Display current rotation angle in degrees next to slider | major  | Showing the angle value helps users know the exact rotation applied.                                             | None         |
| 12  | layout      | Position angle display next to the slider                | minor  | Placing angle next to slider keeps the rotation value near its control.                                          | None         |

## Justification

The application achieved a 91.67% pass rate with one specific failure. An upload button allows users to load an image, which displays on a canvas. A slider labeled "Rotation" with range 0 to 360 degrees appears below the canvas with a default value of 0. The slider stores the current rotation angle. As users drag the slider, the image rotates in real-time to match the slider angle. The current rotation angle displays in degrees. However, the model failed to position the angle display next to the slider. Instead, the angle appears below the slider in a separate row or above the canvas in a header, not next to the slider as required. This positioning issue caused the failure despite all other functionality working correctly.
