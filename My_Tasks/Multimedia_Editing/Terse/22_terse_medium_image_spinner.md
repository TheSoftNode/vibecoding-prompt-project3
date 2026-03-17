Category: Multimedia_Editing

Prompt style: Terse

Title: Image Transform Tool

Prompt: Upload image. Rotate with angle slider. Scale with size slider. Flip horizontal and vertical with buttons. Download result.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                 | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for image                             | major  | The upload button lets users select an image to transform.                                                       | None         |
| 2   | interaction | Display uploaded image on canvas after user uploads         | major  | Showing the image lets users see what they're transforming.                                                      | None         |
| 3   | visual      | Display angle slider for rotation                           | major  | The angle slider gives users control to rotate the image to different angles.                                    | None         |
| 4   | interaction | Rotate image when angle slider moves                        | major  | Rotating the image creates the rotation transformation effect.                                                   | C3           |
| 5   | visual      | Display size slider for scaling                             | major  | The size slider gives users control to resize the image.                                                         | None         |
| 6   | interaction | Scale image when size slider moves                          | major  | Scaling the image changes its dimensions.                                                                        | C5           |
| 7   | state       | Keep image visible during transformations                   | major  | The image must stay visible while transforming so users can see the changes.                                     | C4, C6       |
| 8   | visual      | Display flip horizontal button                              | major  | The flip horizontal button lets users mirror the image left to right.                                            | None         |
| 9   | interaction | Flip image horizontally when button clicked                 | major  | Clicking flips the image along the vertical axis creating a mirror effect.                                       | C8           |
| 10  | visual      | Display flip vertical button                                | major  | The flip vertical button lets users mirror the image top to bottom.                                              | None         |
| 11  | interaction | Flip image vertically when button clicked                   | major  | Clicking flips the image along the horizontal axis creating an upside-down effect.                               | C10          |
| 12  | visual      | Display download button                                     | major  | The download button lets users save their transformed image.                                                     | None         |
| 13  | interaction | Download result when button clicked                         | major  | Clicking download exports the current canvas state as an image file.                                             | C12          |

## Justification

The Image Transform Tool allows users to rotate, scale, and flip images with simple controls. Users upload an image which displays on a canvas. An angle slider rotates the image and a size slider scales it. Flip horizontal and flip vertical buttons mirror the image along different axes. The image stays visible during all transformations. A download button exports the transformed result as an image file.
