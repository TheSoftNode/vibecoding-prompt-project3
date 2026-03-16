Category: Multimedia_Editing

Prompt style: Casual

Title: Image Kaleidoscope

Prompt: Need a kaleidoscope effect maker for images. Show a file upload button labeled "Upload Image" at the top. Load the tool with a default kaleidoscope pattern showing 6 triangular sections in different solid colors arranged in a circle. When I upload a new image, replace the kaleidoscope pattern with the uploaded image transformed into the same 6-section kaleidoscope style.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display file upload button                               | major  | Users need a way to select their own images to transform into kaleidoscopes.       | None         |
| 2  | layout      | Position upload button at the top                        | minor  | Placing the control at the top makes it easy to find when users first open the tool. | C1           |
| 3  | content     | Label button "Upload Image"                              | minor  | A clear label helps users understand what the button does without guessing.        | C1           |
| 4  | state       | Load tool with default kaleidoscope pattern              | minor  | Showing a default pattern on load demonstrates what the tool does right away.      | None         |
| 5  | visual      | Display 6 triangular sections in different solid colors  | major  | Colored sections make the kaleidoscope structure visually clear and appealing.     | None         |
| 6  | layout      | Arrange the 6 sections in a circle                       | major  | Circular arrangement creates the classic kaleidoscope look users expect.           | C5           |
| 7  | interaction | Replace pattern with uploaded image when user uploads    | major  | Replacing the pattern lets users see their own photos transformed instantly.       | None         |
| 8  | interaction | Transform uploaded image into 6-section kaleidoscope     | major  | Applying the same 6-section style keeps the kaleidoscope effect consistent.        | None         |

## Justification

The Image Kaleidoscope works as expected with a default colored pattern. The tool loads with a default kaleidoscope pattern showing 6 triangular sections in different solid colors arranged in a circular pattern. An "UPLOAD IMAGE" button labeled "Upload Image" displays at the top of the interface. When users upload a new image, the kaleidoscope pattern gets replaced with the uploaded image transformed into the same 6-section kaleidoscope style.
