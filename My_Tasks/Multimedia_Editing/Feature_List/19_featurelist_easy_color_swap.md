Category: Multimedia_Editing

Prompt style: Feature_List

Title: Image Edge Trace

Prompt: Build an image edge tracer that extracts outlines from uploaded images. Display an upload button labeled "Upload Image" at the top of the page. When users upload an image, show it on a canvas in full color. Below the canvas, display an "Extract Edges" button. When users click the Extract Edges button, apply edge detection to identify boundaries and outlines in the image, then convert the displayed image to show only the detected edges as black lines on a white background, creating a sketch-like outline version where shapes and boundaries are highlighted.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                                  | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button                                            | major  | The upload button helps users bring their image into the edge tracer for outline extraction.                               | None         |
| 2   | layout      | Position upload button at top of page                            | minor  | Positioning at the top makes the upload button easy to find so users can start edge extraction quickly.                    | C1           |
| 3   | content     | Label upload button "Upload Image"                               | minor  | The label clearly identifies the button's purpose for selecting image files.                                               | C1           |
| 4   | visual      | Display canvas                                                   | major  | The canvas provides a rendering surface for displaying the original and edge-traced images.                                | None         |
| 5   | interaction | Display uploaded image on canvas after user uploads             | major  | Showing the image after upload lets users see what they uploaded before edge extraction begins.                            | C1           |
| 6   | state       | Display uploaded image in full color                             | minor  | Full color display maintains the original image state showing all details before conversion to edge outline.               | C5           |
| 7   | visual      | Display "Extract Edges" button                                   | major  | The extract edges button gives users the control to trigger the edge detection process.                                    | None         |
| 8   | layout      | Position "Extract Edges" button below canvas                     | minor  | Placing the button below the canvas creates clear workflow from viewing to action.                                         | C4, C7       |
| 9   | content     | Label button "Extract Edges"                                     | minor  | The label communicates what action the button performs.                                                                    | C7           |
| 10  | interaction | Apply edge detection when button is clicked                      | major  | Clicking the button triggers the edge detection algorithm that processes the image.                                        | C7           |
| 11  | state       | Identify boundaries and outlines in the image                    | major  | Edge detection analyzes the image to locate boundaries and shape outlines for extraction.                                  | C10          |
| 12  | state       | Convert image to show only detected edges                        | major  | Conversion removes color and texture, displaying only the extracted edge information.                                      | C11          |
| 13  | visual      | Display edges as black lines on white background                 | major  | Black lines on white background creates clear contrast showing the detected edges as a sketch-like outline.                | C12          |
| 14  | state       | Highlight shapes and boundaries in edge version                  | major  | Highlighting boundaries emphasizes the structural elements of the original image in the outline form.                      | C12          |

## Justification

The image edge tracer works as an outline extraction tool that converts photos to sketch-like line drawings. An upload button displays at the top of the page. When users upload an image, it appears on a canvas in full color showing the original image. Below the canvas, an "Extract Edges" button displays. When users click the Extract Edges button, the tool detects edges and boundaries in the image using edge detection algorithms. The canvas then displays only the detected edges as black lines on a white background, creating a sketch-like outline version where boundaries and shapes are highlighted. This transformation emphasizes the structural elements of the original image in a minimalist line art form.
