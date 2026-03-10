Category: Multimedia Editing

Prompt style: Conversational

Title: Pixel Art Generator with Palette Extractor

Prompt: I need to convert regular photos into pixel art style. Upload an image to display it on a canvas. Add a pixelation slider ranging from 4x4 to 32x32 pixels that controls the block size - as I move the slider, the image pixelates in real-time showing larger or smaller pixel blocks. Below the canvas, automatically extract and display the 5 most dominant colors from the pixelated image as color swatches showing the hex code under each swatch. Include a "Download Pixel Art" button that saves the pixelated canvas as a PNG file.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                                         | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for image file                             | major  | The upload button lets users select photos they want to convert to pixel art.                                                     | None         |
| 2   | interaction | Display uploaded image on canvas when file is selected           | major  | Loading the image onto canvas enables the pixelation processing to begin.                                                         | C1           |
| 3   | visual      | Display pixelation slider ranging from 4x4 to 32x32              | major  | The slider gives users control over how blocky or detailed the pixel art should be.                                               | None         |
| 4   | state       | Calculate pixel block size based on slider value                 | major  | Block size calculation determines how many pixels get averaged into each art block.                                               | None         |
| 5   | interaction | Pixelate image in real-time as slider moves                      | major  | Real-time pixelation lets users immediately see the effect of different block sizes.                                              | C3           |
| 6   | content     | Display current pixelation value (e.g. "16x16") near slider     | minor  | Showing the exact block size helps users understand the current pixelation level.                                                 | None         |
| 7   | state       | Extract 5 most dominant colors from pixelated image              | major  | Color extraction analyzes the pixelated image to find the most frequently used colors.                                            | None         |
| 8   | visual      | Display 5 color swatches below canvas                            | major  | Color swatches visually show the dominant palette extracted from the pixel art.                                                   | C7           |
| 9   | content     | Display hex code under each color swatch                         | major  | Hex codes let users copy the exact color values for use in their own projects.                                                    | C8           |
| 10  | layout      | Position color swatches below the canvas                         | minor  | Placing swatches below keeps them visible without covering the pixel art preview.                                                 | None         |
| 11  | visual      | Display "Download Pixel Art" button                              | major  | The download button gives users a way to save their pixelated creation.                                                           | None         |
| 12  | interaction | Save pixelated canvas as PNG when download button is clicked     | major  | Downloading captures the pixel art so users can use it in games or digital artwork.                                               | C11          |

## Justification

The pixel art generator converts regular photos into retro-style pixel art with color palette analysis. Users upload an image which displays on a canvas. A pixelation slider ranging from 4x4 to 32x32 controls the pixel block size, with real-time updates as the slider moves showing the current value (like "16x16"). The tool automatically extracts the 5 most dominant colors from the pixelated image and displays them as color swatches below the canvas, each showing its hex code underneath for easy copying. A "Download Pixel Art" button saves the pixelated canvas as a PNG file for use in game design, digital art projects, or social media posts.
