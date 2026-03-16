Category: Multimedia_Editing

Prompt style: Terse

Title: Photo Collage Grid

Prompt: Upload 4 images. Arrange in 2x2 grid with 20px gaps. Drag each image to swap positions. Border width slider. Download grid as one image.

Required libraries: react, tailwindcss, lucide-react, html2canvas

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for 4 images                    | major  | The upload button lets users select their 4 photos to create the collage.                                        | None         |
| 2   | interaction | Display all 4 uploaded images after user uploads      | major  | Showing all 4 images lets users see what photos are in the collage before arranging.                             | None         |
| 3   | layout      | Arrange images in 2x2 grid                            | major  | The 2x2 grid creates the classic four-photo collage layout users expect.                                         | C2           |
| 4   | layout      | Display 20px gaps between images                      | minor  | Gaps separate the images visually so each photo is distinct in the grid.                                         | C3           |
| 5   | interaction | Swap image positions when user drags an image         | major  | Dragging to swap lets users rearrange photos to get their preferred layout.                                      | None         |
| 6   | state       | Maintain all 4 images visible after drag swap         | major  | Images must stay visible during rearrangement so users can see the new layout.                                   | C5           |
| 7   | visual      | Display border width slider                           | major  | The slider gives users control over how thick the borders around images should be.                               | None         |
| 8   | state       | Apply border width to all images based on slider      | major  | Changing border width lets users customize the collage appearance.                                               | C7           |
| 9   | visual      | Display download button                               | major  | The download button lets users save their finished collage as a single image file.                               | None         |
| 10  | interaction | Download grid as one combined image when button clicked | major  | Downloading combines all 4 images into one file for easy sharing.                                                | None         |
| 11  | layout      | Maintain 2x2 grid structure in downloaded image       | minor  | The downloaded image must preserve the grid layout users arranged.                                               | C10          |
| 12  | state       | Keep 20px gaps visible in downloaded image            | minor  | Gaps must remain in the final image to match what users see on screen.                                           | C10          |

## Justification

The Photo Collage Grid allows users to create a 2x2 photo collage with customizable borders. An upload button lets users select 4 images which display in a 2x2 grid with 20px gaps between them. Users can drag any image to swap positions with another, and all 4 images remain visible after the swap. A border width slider controls the thickness of borders around all images. A download button exports the entire grid as one combined image, maintaining the 2x2 structure and 20px gaps in the final file.
