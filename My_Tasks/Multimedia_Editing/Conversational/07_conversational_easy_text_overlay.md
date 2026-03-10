Category: Multimedia Editing

Prompt style: Conversational

Title: Image Text Overlay Editor

Prompt: I need to add text to images. Show an upload button labeled "Upload Image" to select an image file. When I upload an image, display it centered on the screen. Below the image, show a text input field. As I type in the input field, the text should appear centered on top of the image in white color, updating with each keystroke.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                                     | Weight | Rationale                                                                                                                                     | Dependent On |
| --- | ----------- | ----------------------------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button                                                                           | major  | The upload button provides the interface element that users click to browse and select image files from their device.                         | None         |
| 2   | content     | Label upload button "Upload Image"                                                              | minor  | The "Upload Image" label clearly communicates the button's purpose to users who want to add images for editing.                              | None         |
| 3   | interaction | Upload and display image when file is selected                                                  | major  | Uploading processes the selected file and loads it into the editor so users can begin adding text overlays.                                  | C1           |
| 4   | visual      | Display uploaded image in the center                                                            | major  | The centered image provides the visual canvas where users will see their text overlay appear.                                                | C3           |
| 5   | layout      | Position uploaded image in the center of the interface                                          | minor  | Centering the image creates balanced composition and makes the editing area the focal point of the interface.                                | None         |
| 6   | visual      | Display text input field below the image                                                        | major  | The input field below the image allows users to type the text they want to overlay without obscuring the image preview.                      | None         |
| 7   | state       | Update text overlay content as user types in the input field                                    | major  | Live updating means the text overlay changes with each keystroke so users immediately see how their text looks on the image.                 | None         |
| 8   | visual      | Display entered text centered on top of the image in white color                                | major  | White text centered on the image ensures the overlay is visible and positioned prominently for most image types.                             | C7           |
| 9   | layout      | Position text centered on top of the image                                                      | minor  | Centering the text overlay horizontally and vertically ensures it appears balanced regardless of the image dimensions or content.             | None         |

## Justification

The image text overlay editor works exactly as expected with image upload and text overlay functionality. An upload button allows selecting an image file, which displays centered on the screen when uploaded. Below the image, a text input field allows typing overlay text. As users type in the input field, the entered text appears centered on top of the image in white color, updating with each keystroke.
