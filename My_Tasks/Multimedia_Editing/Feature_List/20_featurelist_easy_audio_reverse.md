Category: Multimedia_Editing

Prompt style: Feature_List

Title: Image Rotation Editor

Prompt: Build an image rotation editor for editing image files. Display a file upload button labeled "Upload Image" at the top of the interface. After a user uploads an image file, display the uploaded image below the upload button at its original orientation. Below the displayed image, show three rotation buttons labeled "Rotate 90° Left", "Rotate 180°", and "Rotate 90° Right" arranged horizontally in a row. When a user clicks any of the rotation buttons, rotate the displayed image by the specified amount in the corresponding direction and update the image display to show the new rotated orientation immediately.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display file upload button                               | major  | Users need a way to upload their image file for editing.                           | None         |
| 2  | layout      | Position upload button at the top of the interface       | minor  | Top positioning makes the upload control easy to find when starting.               | C1           |
| 3  | content     | Label button "Upload Image"                              | minor  | A clear label helps users know what file type to upload.                           | C1           |
| 4  | visual      | Display uploaded image                                   | major  | Showing the image lets users see what they are editing.                            | None         |
| 5  | layout      | Position image below upload button                       | minor  | Positioning below the upload button creates a clear top-to-bottom flow.            | C1, C4       |
| 6  | layout      | Display image at original orientation                    | minor  | Original orientation shows the image in its initial unrotated position.            | C4           |
| 7  | visual      | Display three rotation buttons below the image           | major  | The rotation buttons provide the controls for rotating the image.                  | None         |
| 8  | layout      | Arrange buttons horizontally in a row                    | minor  | Horizontal arrangement creates clear side-by-side layout.                          | C7           |
| 9  | content     | Label buttons "Rotate 90° Left", "Rotate 180°", "Rotate 90° Right" | major  | The labels tell users which rotation each button applies.                          | None         |
| 10 | interaction | Rotate image when rotation button clicked                | major  | Clicking rotates the image to the new orientation.                                 | None         |
| 11 | state       | Rotate image by specified amount in corresponding direction | major  | The rotation transformation applies the correct degree change to the image.        | None         |
| 12 | state       | Update image display to show new rotated orientation     | major  | The updated image shows the rotation result visually.                              | None         |

## Justification

The Image Rotation Editor works as expected for editing image files. A file upload button labeled "Upload Image" displays at the top of the interface. After uploading an image file, the uploaded image displays below the upload button at its original orientation. Below the displayed image, three rotation buttons appear labeled "Rotate 90° Left", "Rotate 180°", and "Rotate 90° Right" arranged horizontally in a row. When users click any of the rotation buttons, the displayed image rotates by the specified amount in the corresponding direction and the image display updates to show the new rotated orientation immediately.
