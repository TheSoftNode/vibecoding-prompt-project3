Category: Multimedia_Editing

Prompt style: One-liner

Title: Image Edge Connector

Prompt: Build an image boundary visualizer.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                 | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | state       | Load tool with default image displayed                      | major  | Loading with a default image shows the boundary visualization effect immediately.                                | None         |
| 2   | visual      | Display loaded image at center of canvas                    | major  | Centering the image creates space around it for boundary lines to canvas edges.                                  | None         |
| 3   | visual      | Draw lines from image edges to canvas edges                 | major  | Lines from image boundaries to canvas boundaries create the visualization effect.                                | None         |
| 4   | layout      | Connect top edge of image to top edge of canvas             | major  | The top connection shows the vertical boundary relationship.                                                     | C3           |
| 5   | layout      | Connect bottom edge of image to bottom edge of canvas       | major  | The bottom connection completes the vertical boundary visualization.                                             | C3           |
| 6   | layout      | Connect left edge of image to left edge of canvas           | major  | The left connection shows the horizontal boundary relationship.                                                  | C3           |
| 7   | layout      | Connect right edge of image to right edge of canvas         | major  | The right connection completes the horizontal boundary visualization.                                            | C3           |
| 8   | visual      | Display upload button for new image                         | major  | The upload button lets users visualize boundaries for their own images.                                          | None         |
| 9   | interaction | Replace image when user uploads new one                     | major  | Replacing the image lets users see boundary visualization for different photos.                                  | None         |
| 10  | state       | Redraw all 4 boundary lines when image changes              | major  | Lines must update to connect the new image's edges to canvas edges.                                              | C9           |
| 11  | state       | Keep image visible after upload                             | major  | The image must stay visible so users see both the image and its boundary connections.                            | C9           |
| 12  | visual      | Display all 4 edge lines simultaneously                     | minor  | All lines must show together to create the complete boundary visualization frame.                                | C3           |

## Justification

The Image Boundary Visualizer draws lines from image edges to canvas boundaries. The tool loads with a default image displayed at the canvas center. Four lines draw from the image edges to the corresponding canvas edges: top edge to top, bottom to bottom, left to left, and right to right, creating a boundary visualization frame. All 4 edge lines display simultaneously. An upload button lets users select a new image. When uploaded, the tool replaces the image and keeps it visible. All 4 boundary lines redraw to connect the new image's edges to the canvas edges, updating the visualization for the different image size.
