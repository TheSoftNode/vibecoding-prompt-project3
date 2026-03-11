Category: Multimedia Editing

Prompt style: Terse

Title: Image Brightness Adjuster

Prompt: Upload image. Display uploaded image. Show slider labeled "Brightness" from -100 to +100, default 0. Dragging slider adjusts image brightness in real-time. Negative values darken, positive values brighten.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for image                       | major  | The upload button is how users get their image into the editor for brightness adjustment.                        | None         |
| 2   | visual      | Display uploaded image on canvas                      | major  | Showing the image lets users see the current brightness and the effect of adjustments.                           | None         |
| 3   | visual      | Display slider control                                | major  | The slider provides the interface for adjusting brightness up or down.                                           | None         |
| 4   | content     | Display label "Brightness" on slider                  | minor  | Labeling clarifies that the slider controls brightness, not contrast or other properties.                        | None         |
| 5   | content     | Display slider range from -100 to +100                | minor  | Showing the range tells users how much they can darken or brighten the image.                                    | None         |
| 6   | state       | Set slider default value to 0                         | minor  | Default 0 means the image starts at its original brightness before any adjustments.                              | None         |
| 7   | state       | Store current brightness value from slider            | major  | Storing the brightness value is necessary to apply the correct adjustment to the image.                          | None         |
| 8   | interaction | Darken image when slider moves to negative values     | major  | Negative values darkening the image lets users reduce brightness for overexposed photos.                         | C3           |
| 9   | interaction | Brighten image when slider moves to positive values   | major  | Positive values brightening the image lets users increase brightness for underexposed photos.                    | C3           |
| 10  | state       | Apply brightness adjustment in real-time as slider drags | major | Real-time adjustment lets users see the effect immediately while dragging instead of waiting until release.      | None         |
| 11  | layout      | Position slider below the image canvas                | minor  | Placing the slider below keeps the editing control near but separate from the image being edited.                | None         |

## Justification

The application achieved a 90.91% pass rate with one specific failure. An upload button allows users to select an image, which then displays on a canvas. A slider labeled "Brightness" shows a range from -100 to +100 with default value 0. The slider stores the current brightness value. As users drag the slider to negative values, the image darkens in real-time. As they drag to positive values, the image brightens in real-time. The brightness adjustment applies continuously while dragging for immediate visual feedback. However, the model failed to position the slider below the image canvas. Instead, the slider appears to the right of the image in a side panel or above it in a toolbar, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
