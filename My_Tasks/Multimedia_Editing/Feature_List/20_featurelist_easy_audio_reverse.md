Category: Multimedia_Editing

Prompt style: Feature_List

Title: Image Rotation Editor

Prompt: Build an image rotation editor for editing image files. Display a file upload button labeled "Upload Image" at the top of the interface. After a user uploads an image file, display the uploaded image below the upload button at its original orientation. Below the displayed image, show three rotation buttons labeled "Rotate 90° Left", "Rotate 180°", and "Rotate 90° Right" arranged horizontally in a row. When a user clicks any of the rotation buttons, rotate the displayed image by the specified amount in the corresponding direction and update the image display to show the new rotated orientation immediately.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                        | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------------------ | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display file upload button                                         | major  | The upload button helps users bring their image file into the editor for rotation.                               | None         |
| 2   | layout      | Position upload button at the top of the interface                 | minor  | Positioning at the top makes the upload button easy to find so users can start editing quickly.                  | C1           |
| 3   | content     | Label button "Upload Image"                                        | minor  | The label communicates what action the button performs and what type of file to select.                          | C1           |
| 4   | interaction | Display uploaded image after user uploads                          | major  | Showing the image after upload lets users see what they uploaded for editing.                                    | None         |
| 5   | layout      | Position image below upload button                                 | minor  | Placing the image below the upload button creates a logical top-down workflow from uploading to editing.         | C1, C4       |
| 6   | state       | Display image at original orientation                              | minor  | Starting with the original orientation gives users a baseline before applying any rotation changes.              | C4           |
| 7   | visual      | Display three rotation buttons                                     | major  | The rotation buttons give users the controls they need to actually rotate the image.                             | None         |
| 8   | layout      | Position buttons below the image                                   | minor  | Placing buttons below the image creates clear workflow from viewing to action.                                   | C4, C7       |
| 9   | layout      | Arrange buttons horizontally in a row                              | minor  | Arranging buttons side by side makes it easy to compare and choose between rotation options.                     | C7           |
| 10  | content     | Label buttons "Rotate 90° Left", "Rotate 180°", "Rotate 90° Right" | major  | Clear button labels tell users exactly how much and in which direction each button will rotate the image.        | None         |
| 11  | interaction | Rotate image when rotation button clicked                          | major  | Clicking a rotation button triggers the rotation action that changes the image orientation.                      | None         |
| 12  | state       | Rotate image by specified amount in corresponding direction        | major  | The rotation calculation must apply the exact degree amount in the correct direction to match user expectations. | None         |
| 13  | state       | Update image display to show new rotated orientation               | major  | After rotation is applied, the display must update to show the new orientation so users can see the result.      | None         |

## Justification

The Image Rotation Editor works as expected for editing image files. A file upload button labeled "Upload Image" displays at the top of the interface. After uploading an image file, the uploaded image displays below the upload button at its original orientation. Below the displayed image, three rotation buttons appear labeled "Rotate 90° Left", "Rotate 180°", and "Rotate 90° Right" arranged horizontally in a row. When users click any of the rotation buttons, the displayed image rotates by the specified amount in the corresponding direction and the image display updates to show the new rotated orientation immediately.
