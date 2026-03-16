Category: Multimedia_Editing

Prompt style: One-liner

Title: Image Comparison Slider

Prompt: Build an image comparison slider.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                 | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for before image                      | major  | Users need to upload the first image to create a before/after comparison.                                        | None         |
| 2   | visual      | Display upload button for after image                       | major  | Users need to upload the second image to complete the comparison pair.                                           | None         |
| 3   | interaction | Display before image when user uploads                      | major  | Showing the before image lets users see the first half of their comparison.                                      | None         |
| 4   | interaction | Display after image when user uploads                       | major  | Showing the after image lets users see the second half of their comparison.                                      | None         |
| 5   | layout      | Position both images overlapping in same area               | major  | Overlapping images creates the comparison effect where slider reveals one or the other.                          | C3, C4       |
| 6   | visual      | Display vertical slider divider                             | major  | The slider provides the control for revealing how much of each image to show.                                    | None         |
| 7   | interaction | Move slider when user drags divider                         | major  | Dragging lets users control the reveal position interactively.                                                   | None         |
| 8   | state       | Clip before image at slider position                        | major  | Clipping the before image reveals the after image on one side of the slider.                                     | C7           |
| 9   | state       | Clip after image at slider position                         | major  | Clipping the after image reveals the before image on the other side of the slider.                               | C7           |
| 10  | state       | Keep both images visible during slider drag                 | major  | Both images must stay visible while dragging so users see the comparison transition smoothly.                    | C7           |
| 11  | layout      | Align both images at same dimensions                        | minor  | Matching dimensions ensures the images line up properly for accurate comparison.                                 | C5           |
| 12  | state       | Set slider default position at center                       | minor  | Starting at center shows equal amounts of both images initially for balanced comparison.                         | None         |

## Justification

The Image Comparison Slider creates a before/after comparison tool where users can interactively reveal portions of two images. Upload buttons for before and after images allow users to select their comparison pair. When uploaded, both images display overlapping in the same area with matching dimensions. A vertical slider divider displays at the center position by default. Users can drag the slider to move its position. As the slider moves, the before image clips at the slider position on one side while the after image clips on the other side, revealing the comparison. Both images remain visible during the drag, creating a smooth transition effect.
