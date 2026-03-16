Category: Multimedia_Editing

Prompt style: Casual

Title: Image Kaleidoscope

Prompt: Need a kaleidoscope effect maker for images. Show a file upload button labeled "Upload Image" at the top. Load the tool with a default sample image showing a colorful kaleidoscope pattern with 6 mirrored triangular sections arranged in a circle. When I upload a new image, replace the kaleidoscope pattern with the uploaded image transformed into the same 6-section kaleidoscope style.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display file upload button                               | major  | Users need a way to select their own images to transform into kaleidoscopes.       | None         |
| 2  | layout      | Position upload button at the top                        | minor  | Placing the control at the top makes it easy to find when users first open the tool. | C1           |
| 3  | content     | Label button "Upload Image"                              | minor  | A clear label helps users understand what the button does without guessing.        | C1           |
| 4  | state       | Load tool with default sample image                      | minor  | Showing a sample kaleidoscope on load demonstrates what the tool does right away.  | None         |
| 5  | visual      | Display colorful kaleidoscope pattern with 6 mirrored sections | major  | A colorful example makes the kaleidoscope effect visually appealing and clear.     | None         |
| 6  | layout      | Arrange sections in a circle                             | major  | Circular arrangement creates the classic kaleidoscope look users expect.           | C5           |
| 7  | interaction | Replace pattern with uploaded image when user uploads    | major  | Replacing the pattern lets users see their own photos transformed instantly.       | None         |
| 8  | interaction | Transform uploaded image into 6-section kaleidoscope     | major  | Applying the same 6-section style keeps the kaleidoscope effect consistent.        | None         |

## Justification

The Image Kaleidoscope works as expected. The tool loads with a default sample image showing a colorful kaleidoscope pattern with 6 mirrored triangular sections arranged in a circle. A file upload button labeled "Upload Image" displays at the top. When users upload a new image, the kaleidoscope pattern gets replaced with the uploaded image transformed into the same 6-section kaleidoscope style.
