Category: Multimedia_Editing

Prompt style: Casual

Title: Image Kaleidoscope

Prompt: Need a kaleidoscope effect maker for images. Show a file upload button labeled "Upload Image" at the top. Load the tool with a default sample image showing a colorful kaleidoscope pattern with 6 mirrored triangular sections arranged in a circle. When I upload a new image, replace the kaleidoscope pattern with the uploaded image transformed into the same 6-section kaleidoscope style.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display file upload button                               | major  | The upload button lets users select their image to transform.                      | None         |
| 2  | layout      | Position upload button at the top                        | minor  | Top positioning makes the upload control easily accessible.                        | C1           |
| 3  | content     | Label button "Upload Image"                              | minor  | The label tells users what the button does.                                        | C1           |
| 4  | state       | Load tool with default sample image                      | major  | Loading with sample data lets users see the kaleidoscope immediately.              | None         |
| 5  | visual      | Display kaleidoscope pattern with 6 mirrored sections    | major  | The 6-section pattern provides the initial kaleidoscope layout.                    | None         |
| 6  | layout      | Arrange sections in a circle                             | major  | Circular arrangement creates the traditional kaleidoscope appearance.              | C5           |
| 7  | interaction | Replace pattern with uploaded image when user uploads    | major  | Image replacement allows users to create kaleidoscopes from their own photos.      | None         |
| 8  | visual      | Transform uploaded image into 6-section kaleidoscope     | major  | The transformation applies the kaleidoscope effect to the new image.               | None         |

## Justification

The Image Kaleidoscope works as expected. The tool loads with a default sample image showing a colorful kaleidoscope pattern with 6 mirrored triangular sections arranged in a circle. A file upload button labeled "Upload Image" displays at the top. When users upload a new image, the kaleidoscope pattern gets replaced with the uploaded image transformed into the same 6-section kaleidoscope style.
