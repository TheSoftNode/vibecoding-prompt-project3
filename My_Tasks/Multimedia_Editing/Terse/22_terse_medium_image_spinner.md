Category: Multimedia_Editing

Prompt style: Terse

Title: Image Rotation Tracer

Prompt: Upload image. Rotate with angle slider. Draw lines from image corners to canvas edges. Show rotation angle label updating in real-time.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                 | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for image                             | major  | The upload button lets users select an image to rotate and trace.                                                | None         |
| 2   | interaction | Display uploaded image on canvas after user uploads         | major  | Showing the image lets users see what they're rotating and tracing.                                              | None         |
| 3   | visual      | Display angle slider for rotation                           | major  | The slider gives users control to rotate the image to different angles.                                          | None         |
| 4   | interaction | Rotate image when slider moves                              | major  | Rotating the image creates different corner positions to trace from.                                             | C3           |
| 5   | state       | Keep image visible during rotation                          | major  | The image must stay visible while rotating so users can see the transformation.                                  | C4           |
| 6   | visual      | Draw lines from image corners to canvas edges               | major  | Lines show the geometric relationship between rotated image corners and canvas boundaries.                       | None         |
| 7   | state       | Update line positions when image rotates                    | major  | Lines must redraw from new corner positions as the image rotates.                                                | C4, C6       |
| 8   | layout      | Connect each of 4 corners to nearest canvas edge            | major  | Connecting to nearest edges creates a dynamic tracing pattern as rotation changes corner positions.              | C6           |
| 9   | content     | Display rotation angle label                                | major  | The label shows users the exact rotation angle in degrees.                                                       | None         |
| 10  | state       | Update angle label in real-time as slider moves             | major  | Real-time updates let users see the angle value change as they drag the slider.                                  | C4           |
| 11  | state       | Calculate correct corner positions after rotation           | major  | Accurate corner calculations ensure lines connect from the right points on rotated image.                        | C4           |
| 12  | visual      | Keep all 4 corner lines visible during rotation             | minor  | All lines must stay visible to show the complete tracing pattern throughout rotation.                            | C7           |

## Justification

The Image Rotation Tracer creates a visual effect showing geometric relationships as images rotate. Users upload an image which displays on a canvas. An angle slider rotates the image, keeping it visible during rotation. As the image rotates, the tool calculates the correct positions of all 4 corners and draws lines from each corner to the nearest canvas edge. The lines update their positions in real-time as rotation changes corner locations. A rotation angle label displays and updates in real-time as users drag the slider, showing the exact degree value. All 4 corner lines remain visible throughout the rotation, creating a dynamic tracing pattern.
