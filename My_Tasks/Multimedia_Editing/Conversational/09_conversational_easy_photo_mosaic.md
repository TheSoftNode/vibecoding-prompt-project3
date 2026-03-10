Category: Multimedia Editing

Prompt style: Conversational

Title: Image Blend Editor

Prompt: I need to build an image blend editor where I can overlay two images and adjust the transparency blend between them. Show two upload zones side by side labeled "Upload Base Image" and "Upload Overlay Image". When I upload both images, display them overlaid on a canvas below, with the overlay image at 50% opacity by default. Below the canvas, show a slider labeled "Overlay Opacity" ranging from 0% to 100%. As I drag the slider, update the overlay image opacity in real-time to blend between the base image and overlay image.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                                         | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload zone for base image                               | major  | Without a way to upload the base image, users can't get their background layer into the editor.                                   | None         |
| 2   | content     | Display label "Upload Base Image" on first upload zone           | minor  | Users need to know which upload zone is for the base so they don't accidentally swap the layer order.                             | C1           |
| 3   | visual      | Display upload zone for overlay image                            | major  | The overlay is the second layer that gets blended on top, so users need a separate upload for it.                                 | None         |
| 4   | content     | Display label "Upload Overlay Image" on second upload zone       | minor  | Clear labeling prevents confusion about which image goes where in the layer stack.                                                | C3           |
| 5   | layout      | Position two upload zones side by side                           | minor  | Placing them side by side visually reinforces that these are two separate layers for blending.                                    | None         |
| 6   | visual      | Display canvas for overlaid images                               | major  | The canvas is where users see the actual blend result and make their editing decisions.                                           | None         |
| 7   | interaction | Display overlaid images on canvas when both images are uploaded  | major  | Users need instant confirmation that their images loaded correctly before they start adjusting the blend.                         | C6           |
| 8   | state       | Set overlay opacity to 50% by default                            | major  | Starting at 50% lets users see both images equally, which is more useful than starting fully opaque or transparent.               | None         |
| 9   | visual      | Display slider for overlay opacity adjustment                    | major  | The slider is the main editing tool that lets users control how much each image shows through.                                    | None         |
| 10  | content     | Display label "Overlay Opacity" with range 0% to 100% on slider  | minor  | Without the label and range, users won't understand what the slider does or what values it covers.                                | C9           |
| 11  | state       | Store current opacity value as slider moves                      | major  | Tracking the opacity value is essential for applying the correct blend amount to the overlay image.                               | None         |
| 12  | interaction | Update overlay opacity on canvas when slider is dragged          | major  | Real-time feedback while dragging lets users see exactly how the blend looks at different opacity levels.                         | C9           |

## Justification

The image blend editor enables users to overlay two images and adjust their transparency blend for creative compositing. Two upload zones positioned side by side, labeled "Upload Base Image" and "Upload Overlay Image", accept the two image layers. When both images are uploaded, they display overlaid on a canvas below with the overlay at 50% opacity by default. A slider labeled "Overlay Opacity" with range 0% to 100% appears below the canvas. As users drag the slider, the overlay opacity updates in real-time on the canvas, allowing them to interactively adjust the blend between fully showing the base image (0%) to fully showing the overlay image (100%).
