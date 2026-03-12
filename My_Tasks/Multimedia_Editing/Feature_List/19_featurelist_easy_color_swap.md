Category: Multimedia_Editing

Prompt style: Feature_List

Title: Dominant Color Swapper

Prompt: Build a dominant color swapper. Upload an image and it displays on a canvas. Below the canvas, show the 3 most dominant colors extracted from the image as colored square swatches with their hex codes. When clicking any swatch, open a color picker to select a replacement color. After selecting a replacement, all pixels matching the original dominant color shift to the new color in real-time on the canvas, updating the image immediately.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for image                           | major  | The upload button lets users choose which image to work with.                                                    | None         |
| 2   | visual      | Display uploaded image on canvas                          | major  | The canvas shows the image so users can see their color changes.                                                 | None         |
| 3   | state       | Extract 3 most dominant colors from image                 | major  | Extracting colors finds the main hues that appear most frequently in the image.                                  | None         |
| 4   | visual      | Display colored square swatches below canvas              | major  | Swatches show users which colors they can replace.                                                               | None         |
| 5   | content     | Display hex code on each color swatch                     | minor  | Hex codes tell users the exact color value of each dominant color.                                               | C3           |
| 6   | interaction | Open color picker when clicking swatch                    | major  | Clicking a swatch lets users choose what new color to swap in.                                                   | None         |
| 7   | state       | Replace all pixels matching original color                | major  | Replacing matching pixels changes every instance of that color across the image.                                 | None         |
| 8   | state       | Shift pixels to new selected color                        | major  | Shifting to the new color creates the color swap effect users expect.                                            | C7           |
| 9   | interaction | Update canvas image in real-time after color selection    | major  | Real-time updates let users see the color change immediately without delay.                                      | C6           |
| 10  | layout      | Position color swatches below canvas                      | minor  | Putting swatches below the image keeps them accessible without covering the canvas.                              | None         |

## Justification

The dominant color swapper works exactly as expected with color extraction and real-time pixel replacement. Users upload an image and it displays on a canvas. Below the canvas, 3 colored square swatches appear showing the most dominant colors extracted from the image, each labeled with its hex code. When users click any swatch, a color picker opens allowing them to select a replacement color. After selecting a new color, all pixels in the image that match the original dominant color instantly shift to the new color, updating the canvas in real-time to show the color swap effect immediately.
