Category: Multimedia_Editing

Prompt style: Feature_List

Title: Image Rotation Editor

Prompt: Build an image rotation editor for editing image files. Display a file upload button labeled "Upload Image" at the top of the interface. After a user uploads an image file, display the uploaded image in a preview area at its original orientation. Below the preview area, show two rotation buttons labeled "Rotate Left" and "Rotate Right" arranged horizontally. When a user clicks any of the rotation buttons, rotate the displayed image 90 degrees in the corresponding direction, keeping the image visible in the preview area while applying the rotation transformation.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                        | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------------------ | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display file upload button                                         | major  | The upload button helps users bring their image file into the editor for rotation.                               | None         |
| 2   | layout      | Position upload button at the top of the interface                 | minor  | Positioning at the top makes the upload button easy to find so users can start editing quickly.                  | C1           |
| 3   | content     | Label button "Upload Image"                                        | minor  | The label communicates what action the button performs and what type of file to select.                          | C1           |
| 4   | interaction | Display uploaded image after user uploads                          | major  | Showing the image after upload lets users see what they uploaded for editing.                                    | None         |
| 5   | layout      | Display image in a preview area                                    | minor  | Placing the image in a preview area provides a dedicated space for viewing the image.                            | C4           |
| 6   | state       | Display image at original orientation                              | minor  | Starting with the original orientation gives users a baseline before applying any rotation changes.              | C4           |
| 7   | visual      | Display two rotation buttons                                       | major  | The rotation buttons give users the controls they need to rotate the image.                                      | None         |
| 8   | layout      | Position buttons below the preview area                            | minor  | Placing buttons below the preview creates clear workflow from viewing to action.                                 | C5, C7       |
| 9   | layout      | Arrange buttons horizontally                                       | minor  | Horizontal arrangement makes both rotation options visible side by side.                                         | C7, C8       |
| 10  | content     | Label buttons "Rotate Left" and "Rotate Right"                     | major  | Clear button labels tell users which direction each button will rotate the image.                                | None         |
| 11  | interaction | Rotate image when rotation button clicked                          | major  | Clicking a rotation button triggers the rotation action that changes the image orientation.                      | None         |
| 12  | state       | Rotate image 90 degrees in corresponding direction                 | major  | The rotation applies 90 degree rotation in the correct direction to match user expectations.                     | None         |
| 13  | state       | Keep image visible in preview area while applying rotation         | major  | The image must remain visible during rotation so users can see the transformation happen.                        | C12          |

## Justification

The Image Rotation Editor works as expected for editing image files. A file upload button labeled "Upload Image" displays at the top of the interface. After uploading an image file, the uploaded image displays in a preview area at its original orientation. Below the preview area, two rotation buttons labeled "Rotate Left" and "Rotate Right" display arranged horizontally. When users click any of the rotation buttons, the displayed image rotates 90 degrees in the corresponding direction, keeping the image visible in the preview area while applying the rotation transformation.
