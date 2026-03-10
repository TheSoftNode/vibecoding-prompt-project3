Category: Multimedia Editing

Prompt style: Conversational

Title: Image Text Overlay Editor

Prompt: I need to add text to images. Show an upload button labeled "Upload Image" at the top. Below it, show a text input field with placeholder "Enter text overlay". When I upload an image, display it centered below the text input. As I type in the input field, store the current text value and display it centered on top of the image in white color, updating with each keystroke.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                                         | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button                                            | major  | The upload button provides the interface element that users click to browse and select image files from their device.             | None         |
| 2   | content     | Label upload button "Upload Image"                               | minor  | The "Upload Image" label clearly communicates the button's purpose to users who want to add images for editing.                   | C1           |
| 3   | layout      | Position upload button at top                                    | minor  | Top positioning makes the upload button the first action in the workflow.                                                         | None         |
| 4   | visual      | Display text input field                                         | major  | The input field is always visible so users can enter text before or after uploading an image.                                     | None         |
| 5   | content     | Display placeholder "Enter text overlay" in input field          | minor  | The placeholder guides users on what to type in the input field.                                                                  | C4           |
| 6   | layout      | Position text input field below upload button                    | minor  | Below positioning creates logical workflow from upload to text entry.                                                             | None         |
| 7   | interaction | Display image centered below text input when file is selected    | major  | Uploading processes the selected file and loads it into the editor so users can begin adding text overlays.                       | C1           |
| 8   | layout      | Position text overlay centered on top of the image               | minor  | Centering the text overlay horizontally and vertically ensures it appears balanced regardless of the image dimensions or content. | None         |
| 9   | state       | Store current text input value                                   | major  | The input value is stored as state and used to render the text that appears on the image.                                         | None         |
| 10  | interaction | Update text overlay display as user types in input field         | major  | Typing triggers live text updates so users immediately see how their text looks on the image with each keystroke.                 | C4           |

## Justification

The image text overlay editor works exactly as expected with image upload and text overlay functionality. An upload button labeled "Upload Image" displays at the top. Below it, a text input field with placeholder "Enter text overlay" is always visible. When an image file is selected, it displays centered below the text input field. As users type in the input field, the current text value is tracked and appears centered on top of the image in white color, updating with each keystroke.
