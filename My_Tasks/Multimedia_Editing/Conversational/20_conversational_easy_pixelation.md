Category: Multimedia_Editing

Prompt style: Conversational

Title: Pixelation Effect Slider

Prompt: I want to create a pixelation effect tool for images. Display a button labeled "Choose Photo" at the top to upload an image. Once uploaded, show the image below the button. Underneath the image, display three preset buttons labeled "Light (5px)", "Medium (15px)", and "Heavy (30px)". When I click a preset button, apply that level of pixelation to the image where larger pixel values create blockier effects. Include a "Save Pixelated Image" button at the bottom to download the result.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display a button at the top                              | major  | The button provides the upload interface for users.                                | None         |
| 2  | content     | Label button "Choose Photo"                              | minor  | The label tells users what file type to select.                                    | C1           |
| 3  | visual      | Display uploaded image below the button                  | major  | The image shows users their photo ready for pixelation.                            | None         |
| 4  | layout      | Position image below upload button                       | minor  | Placing image below creates a logical top-to-bottom flow.                          | C3           |
| 5  | visual      | Display three preset buttons underneath image            | major  | The preset buttons provide quick pixelation intensity options.                     | None         |
| 6  | content     | Label buttons "Light (5px)", "Medium (15px)", and "Heavy (30px)" | major  | The labels tell users the pixel size each preset applies.                          | C5           |
| 7  | interaction | Apply pixelation when preset button clicked              | major  | Applying pixelation creates the visual effect users want.                          | None         |
| 8  | visual      | Display "Save Pixelated Image" button at the bottom      | major  | The save button lets users download their pixelated result.                        | None         |
| 9  | interaction | Download pixelated image when button clicked             | major  | Downloading provides the final output for users to use elsewhere.                  | None         |

## Justification

The Pixelation Effect tool works as expected with preset intensity options. A button labeled "Choose Photo" displays at the top for users to upload an image. Once uploaded, the image appears below the button. Underneath the image, three preset buttons display labeled "Light (5px)", "Medium (15px)", and "Heavy (30px)". When users click a preset button, that level of pixelation applies to the image where larger pixel values create blockier effects. A "Save Pixelated Image" button at the bottom allows users to download the result.
