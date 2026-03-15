Category: SVG Generation

Prompt style: Conversational

Title: Custom Stamp Seal Generator

Prompt: I want to create circular stamp seals. Type text into an input field and pick a color. Click "Generate Stamp" to create an SVG circular seal with the text curved around the border and a star in the center, using the selected color. Add a "Download SVG" button to save it.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                                        | Weight | Rationale                                                                                            | Dependent On |
| --- | ----------- | -------------------------------------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display a text input field                                                                        | major  | The input field collects text for the stamp border.                                                  | None         |
| 2   | visual      | Display a color picker                                                                            | major  | The color picker lets users customize the stamp color.                                               | None         |
| 3   | visual      | Display a "Generate Stamp" button                                                                 | major  | The button triggers stamp creation.                                                                  | None         |
| 4   | interaction | Create an SVG circular seal when the Generate Stamp button is clicked                             | major  | Clicking initiates the stamp generation.                                                             | None         |
| 5   | state       | Calculate curved text path positioning around the circle border                                   | major  | Computing positions places each character correctly along the curve.                                 | C4           |
| 6   | visual      | Display the input text curved around the circle border as SVG                                     | major  | Curved text creates the authentic stamp seal appearance.                                             | C5           |
| 7   | layout      | Position the star icon in the center of the circle                                                | minor  | Center placement creates the focal point of the stamp.                                               | C4           |
| 8   | visual      | Apply the selected color to the stamp elements                                                    | major  | Using the chosen color customizes the stamp appearance.                                              | C4           |
| 9   | content     | Label the download button "Download SVG"                                                           | minor  | The label identifies the export function.                                                            | None         |
| 10  | interaction | Download the stamp as SVG file when the Download SVG button is clicked                            | major  | Clicking saves the generated stamp.                                                                  | C4           |

## Justification

The custom stamp seal generator works exactly as expected. Users type text into the input field and pick a color. Clicking "Generate Stamp" creates an SVG circular seal with the text curved around the border and a star in the center, all in the selected color. The "Download SVG" button saves the stamp as an SVG file.
