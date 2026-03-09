Category: Multimedia Editing

Prompt style: Conversational

Title: Image Text Overlay Editor

Prompt: I need to add text to images. Upload an image that displays in the center. Below the image, show a text input field. When I type text, it appears centered on top of the image in white color. Show a color picker to change the text color. At the bottom, show a "Download Image" button that saves the image with the text overlay.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                                     | Weight | Rationale                                                                                             | Dependent On |
| --- | ----------- | ----------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for image                                                                 | major  | The upload button provides the interface for selecting images to edit.                                | None         |
| 2   | interaction | Upload and display image when file is selected                                                  | major  | Uploading loads the image into the editor for text overlay editing.                                   | C1           |
| 3   | visual      | Display uploaded image in the center                                                            | major  | The image provides the canvas for adding text overlay.                                                | C2           |
| 4   | layout      | Position uploaded image in the center of the interface                                          | minor  | Center positioning makes the image prominently displayed for editing.                                 | None         |
| 5   | visual      | Display text input field below the image                                                        | major  | The input field allows users to type the text they want to overlay on the image.                      | None         |
| 6   | layout      | Position text input field below the image                                                       | minor  | Below-image placement creates natural workflow after image upload.                                    | None         |
| 7   | interaction | Display entered text centered on top of the image in white color when user types                | major  | Live text overlay shows the text appearing on the image as users type.                                | None         |
| 8   | visual      | Display color picker                                                                            | major  | The color picker provides the interface for changing text color.                                      | None         |
| 9   | interaction | Change text color on the image when new color is selected                                       | major  | Color changing updates the overlay text to match the selected color.                                  | None         |
| 10  | content     | Display "Download Image" button label                                                           | minor  | The button label identifies the download functionality.                                               | None         |
| 11  | layout      | Position "Download Image" button at the bottom                                                  | minor  | Bottom placement separates the action button from editing controls.                                   | None         |
| 12  | interaction | Download image with text overlay when Download Image button is clicked                          | major  | Downloading saves the final image with the text overlay applied.                                      | None         |

## Justification

The image text overlay editor works exactly as expected with image upload and text overlay functionality. An upload button allows selecting an image file, which displays in the center of the interface when uploaded. Below the image, a text input field labeled "Enter text" allows typing overlay text. As users type, the entered text appears centered on top of the image in white color. Below the text input, a color picker allows changing the text color, which updates the text on the image immediately. At the bottom, a "Download Image" button saves the image with the text overlay applied.
