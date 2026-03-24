Category: Multimedia_Editing

Prompt style: Feature_List

Title: Image Edge Trace

Prompt: Build an image edge tracer that extracts outlines from uploaded images. Display an upload button at the top of the page. When users upload an image, show it on a canvas in full color. Below the canvas, display an "Extract Edges" button. When users click the button, convert the image to show only the detected edges as black lines on a white background, creating a sketch-like outline version of the original image where boundaries and shapes are highlighted.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                                  | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button                                            | major  | The upload button helps users bring their image into the edge tracer for outline extraction.                               | None         |
| 2   | layout      | Position upload button at top of page                            | minor  | Positioning at the top makes the upload button easy to find so users can start edge extraction quickly.                    | C1           |
| 3   | visual      | Display canvas                                                   | major  | The canvas provides a rendering surface for displaying the original and edge-traced images.                                | None         |
| 4   | interaction | Display uploaded image on canvas after user uploads             | major  | Showing the image after upload lets users see what they uploaded before edge extraction begins.                            | C1           |
| 5   | content     | Display uploaded image in full color                             | minor  | Full color display shows the original image before conversion to edge outline.                                             | C4           |
| 6   | visual      | Display "Extract Edges" button                                   | major  | The extract edges button gives users the control to trigger the edge detection process.                                    | None         |
| 7   | layout      | Position "Extract Edges" button below canvas                     | minor  | Placing button below the canvas creates clear workflow from viewing to action.                                             | C3, C6       |
| 8   | content     | Label button "Extract Edges"                                     | minor  | The label communicates what action the button performs.                                                                    | C6           |
| 9   | interaction | Convert image to edge outline when button is clicked             | major  | Clicking the button triggers the edge detection algorithm that creates the sketch effect.                                  | C6           |
| 10  | state       | Detect edges and boundaries in the image                         | major  | Edge detection identifies the outlines and shapes within the image for extraction.                                         | C9           |
| 11  | visual      | Display edges as black lines on white background                 | major  | Black lines on white background creates clear contrast showing the detected edges as a sketch-like outline.                | C10          |
| 12  | state       | Highlight boundaries and shapes in edge version                  | major  | Highlighting boundaries emphasizes the structural elements of the original image in outline form.                          | C10          |

## Justification

The image edge tracer works as an outline extraction tool that converts photos to sketch-like line drawings. An upload button displays at the top of the page. When users upload an image, it appears on a canvas in full color showing the original image. Below the canvas, an "Extract Edges" button displays. When users click the Extract Edges button, the tool detects edges and boundaries in the image using edge detection algorithms. The canvas then displays only the detected edges as black lines on a white background, creating a sketch-like outline version where boundaries and shapes are highlighted. This transformation emphasizes the structural elements of the original image in a minimalist line art form.
