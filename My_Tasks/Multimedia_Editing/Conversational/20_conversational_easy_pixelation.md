Category: Multimedia_Editing

Prompt style: Conversational

Title: Pixelation Effect Slider

Prompt: I want to create a pixelation effect tool for images. Display a button labeled "Choose Photo" at the top to upload an image. Once uploaded, show the image below the button. Underneath the image, display a horizontal slider labeled "Pixel Size" ranging from 1 to 50. As I drag the slider, apply pixelation to the image in real-time where larger values create blockier pixel effects. Display the current pixel size value as a number next to the slider. Include a "Save Pixelated Image" button at the bottom to download the result.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display a button at the top                              | major  | The button provides the upload interface for users.                                | None         |
| 2  | content     | Label button "Choose Photo"                              | minor  | The label tells users what file type to select.                                    | C1           |
| 3  | visual      | Display uploaded image below the button                  | major  | The image shows users their photo ready for pixelation.                            | None         |
| 4  | layout      | Position image below upload button                       | minor  | Placing image below creates a logical top-to-bottom flow.                          | C3           |
| 5  | visual      | Display horizontal slider underneath image               | major  | The slider provides the pixelation intensity control.                              | None         |
| 6  | content     | Label slider "Pixel Size"                                | minor  | The label tells users what the slider adjusts.                                     | C5           |
| 7  | state       | Set slider range from 1 to 50                            | major  | The 1-50 range provides variation from subtle to heavy pixelation.                 | None         |
| 8  | interaction | Apply pixelation to image in real-time as slider drags   | major  | Real-time updates let users see the effect as they adjust intensity.               | None         |
| 9  | visual      | Display current pixel size value as number next to slider | major  | The number shows users the exact pixelation level.                                 | None         |
| 10 | layout      | Position pixel size value next to slider                 | minor  | Placing value next to slider creates clear association.                            | C9           |
| 11 | visual      | Display "Save Pixelated Image" button at the bottom      | major  | The save button lets users download their pixelated result.                        | None         |
| 12 | interaction | Download pixelated image when button clicked             | major  | Downloading provides the final output for users to use elsewhere.                  | None         |

## Justification

The Pixelation Effect Slider works as expected with real-time intensity adjustment. A button labeled "Choose Photo" displays at the top for users to upload an image. Once uploaded, the image appears below the button. Underneath the image, a horizontal slider labeled "Pixel Size" displays ranging from 1 to 50. As users drag the slider, pixelation applies to the image in real-time where larger values create blockier pixel effects. The current pixel size value displays as a number next to the slider. A "Save Pixelated Image" button at the bottom allows users to download the result.
