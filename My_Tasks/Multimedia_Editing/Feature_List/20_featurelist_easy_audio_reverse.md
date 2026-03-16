Category: Multimedia_Editing

Prompt style: Feature_List

Title: Image Blur Editor

Prompt: Build an image blur editor for editing image files. Display a file upload button labeled "Upload Image" at the top of the interface. After a user uploads an image file, display the uploaded image in a preview area with no blur applied. Below the preview area, show a slider labeled "Blur Intensity" with range 0 to 100 and default value 0. When a user drags the slider, apply blur effect to the displayed image based on the slider value, keeping the image visible in the preview area while applying the blur transformation.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                | Weight | Rationale                                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display file upload button                                 | major  | The upload button helps users bring their image file into the editor for blur editing.              | None         |
| 2   | layout      | Position upload button at the top of the interface         | minor  | Positioning at the top makes the upload button easy to find so users can start editing quickly.     | C1           |
| 3   | content     | Label button "Upload Image"                                | minor  | The label communicates what action the button performs and what type of file to select.             | C1           |
| 4   | interaction | Display uploaded image after user uploads                  | major  | Showing the image after upload lets users see what they uploaded for editing.                       | None         |
| 5   | layout      | Display image in a preview area                            | minor  | Placing the image in a preview area provides a dedicated space for viewing the image.               | C4           |
| 6   | state       | Display image with no blur applied initially               | minor  | Starting with no blur gives users a baseline before applying any blur effect.                       | C4           |
| 7   | visual      | Display blur intensity slider                              | major  | The slider gives users the control they need to adjust the blur effect.                             | None         |
| 8   | layout      | Position slider below the preview area                     | minor  | Placing slider below the preview creates clear workflow from viewing to action.                     | C5, C7       |
| 9   | content     | Label slider "Blur Intensity"                              | minor  | The label communicates what the slider controls.                                                    | C7           |
| 10  | content     | Display slider range from 0 to 100                         | minor  | Showing the range tells users the minimum and maximum blur intensity values.                        | C7           |
| 11  | state       | Set slider default value to 0                              | minor  | Default 0 means the image starts with no blur applied.                                              | C7           |
| 12  | interaction | Apply blur effect when user drags slider                   | major  | Dragging the slider applies blur based on the selected intensity value.                             | C7           |
| 13  | state       | Keep image visible in preview area while applying blur     | major  | The image must remain visible during blur application so users can see the transformation happen.   | C12          |

## Justification

The Image Blur Editor works as expected for editing image files. A file upload button labeled "Upload Image" displays at the top of the interface. After uploading an image file, the uploaded image displays in a preview area with no blur applied initially. Below the preview area, a slider labeled "Blur Intensity" displays with range 0 to 100 and default value 0. When users drag the slider, the tool applies blur effect to the displayed image based on the slider value, keeping the image visible in the preview area while applying the blur transformation.
