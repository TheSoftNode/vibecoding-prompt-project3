Category: Multimedia_Editing

Prompt style: Casual

Title: Image Kaleidoscope

Prompt: Need a kaleidoscope effect maker for images. Show a file upload button labeled "Upload Image" at the top. Load the tool with a default sample image showing a colorful kaleidoscope pattern with 6 mirrored triangular sections arranged in a circle. Below the kaleidoscope, show three preset buttons labeled "Simple (4)", "Classic (6)", and "Complex (8)". When I click a preset button, update the kaleidoscope pattern to show that many mirrored sections. When I upload a new image, replace the kaleidoscope pattern with the uploaded image.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display file upload button at the top                    | major  | The upload button lets users select their image to transform.                      | None         |
| 2  | content     | Label button "Upload Image"                              | minor  | The label tells users what the button does.                                        | None         |
| 3  | state       | Load tool with default sample image                      | major  | Loading with sample data lets users see the kaleidoscope immediately.              | None         |
| 4  | visual      | Display kaleidoscope pattern with 6 mirrored sections    | major  | The 6-section pattern provides the initial kaleidoscope layout.                    | None         |
| 5  | layout      | Arrange sections in a circle                             | major  | Circular arrangement creates the traditional kaleidoscope appearance.              | None         |
| 6  | visual      | Display three preset buttons below kaleidoscope          | major  | The preset buttons provide quick options for pattern complexity.                   | None         |
| 7  | content     | Label buttons "Simple (4)", "Classic (6)", and "Complex (8)" | major  | The labels tell users how many sections each preset creates.                       | None         |
| 8  | interaction | Update kaleidoscope pattern when preset button clicked   | major  | Pattern updates let users see different section variations.                        | None         |
| 9  | interaction | Replace pattern with uploaded image when user uploads    | major  | Image replacement allows users to create kaleidoscopes from their own photos.      | None         |

## Justification

The Image Kaleidoscope works as expected with preset pattern options. The tool loads with a default sample image showing a colorful kaleidoscope pattern with 6 mirrored triangular sections arranged in a circle. A file upload button labeled "Upload Image" displays at the top. Below the kaleidoscope, three preset buttons appear labeled "Simple (4)", "Classic (6)", and "Complex (8)". When users click a preset button, the kaleidoscope pattern updates to show that many mirrored sections. When users upload a new image, the kaleidoscope pattern gets replaced with the uploaded image.
